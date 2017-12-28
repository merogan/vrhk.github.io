---

layout: post
category: C7WAKBTB8
title: "Import AI: #74: Why Uber is betting on evolution, what Facebook and Baidu think about datacenter-scale AI computing, and why Tacotron 2 means speech will soon be spoofable"
date: 2017-12-28 08:24:06
link: http://bit.ly/2pNKOME
image: 
domain: jack-clark.net
author: "Jack Clark"
icon: https://s0.wp.com/i/webclip.png
excerpt: "All hail the new &lsquo;datacenter scale&rsquo; era for AI:&hellip;Facebook Research Paper goes through some of the many problems that come with running AI at the scale of an entire datacenter&hellip;Facebook has published an analysis of how it runs its worldwide fleet of AI services and how its scale has influenced the way it has deployed AI into production. The company uses both CPUs and GPUs, with GPUs being used for large-scale face recognition, language translation, and the &lsquo;Lumos&rsquo; feature-analysis service. It also runs a significant amount of work on CPUs; one major workload is ranking features for newsfeed. &ldquo;Computer vision represents only a small fraction&rdquo; of the total work, Facebook writes.&nbsp;&nbsp;Split languages: Facebook uses &lsquo;Caffe2&rsquo; for its production systems, while its researchers predominantly use PyTorch. Though the company&rsquo;s main ML services (FBLearner Feature Store / FBLearner Flow / FBLearner Predictor) support a bunch of different AI frameworks, they&rsquo;ve all been specially integrated with Caffe2, the company says. &nbsp;&nbsp;The big get bigger: Facebook, like other major AI users, is experimenting with running significantly larger AI models at larger scales: this has altered how it places and networks together its GPU servers, as well as directed it to spin-up research in areas like low-precision training. They&rsquo;re also figuring out ways to use the scale to their advantage. &ldquo;Using certain hyperparameter settings, we can train our image classification models to very large mini-batches, scaling to 256+ GPUs,&rdquo; they write. &ldquo;For one of our larger workloads, data parallelism has been demonstrated to provide 4x the throughput using 5x the machine count (e.g., for a family of models that trains over 4 days, a pool of machines training 100 different models could now train 20 models per day, so training throughput drops by 20%, but the wait time for potential engineering advancement improves from four days to one day).&rdquo; &nbsp;&nbsp;One GPU region to train them all: When Facebook was first experimenting with GPUs for deep learning it rolled out GPUs in a single data center region, which it figured was a good decision as the designs of the servers were changing and the teams needed to become used to maintaining them. This Had some pretty negative consequences down the road, causing a re-think of how the company distributed its data center resources and its infrastructure.Read more: Applied Machine Learning at Facebook: A Datacenter Infrastructure Perspective.
Baidu publishes some rules-of-thumb for how model size relates to performance:&hellip;The beginnings of a theory for deep learning&hellip;Deep learning is an empirical science &ndash; we don&rsquo;t fully understand how various attributes of our neural networks dictate their ultimate representational capacity. That means the day-to-day work of any AI organization involves a lot of empirical experimentation. Now, researchers with Baidu have attempted to formalize some of their ideas about how the scale of a deep learning model relates to its performance. &nbsp;&nbsp;&ldquo;Through empirical testing, we find predictable accuracy scaling as long as we have enough data and compute power to train large models. These results hold for a broad spectrum of state-of-the-art models over four application domains: machine translation, language modeling, image classification, and speech recognition,&rdquo; they write.&nbsp; The results suggest that once researchers get a model to a certain threshold of accuracy they can be confident that by simply adding computer &amp;/or data they can reach x performance within a rough margin of error. &ldquo;Model error improves starting with &ldquo;best guessing&rdquo; and following the power-law curve down to &ldquo;irreducible error&rdquo;,&rdquo; they say. &ldquo;We find that models transition from a small training set region dominated by best guessing to a region dominated by power-law scaling. With sufficiently large training sets, models will saturate in a region dominated by irreducible error (e.g., Bayes error).&rdquo; &nbsp;&nbsp;The insight is useful but still requires experimental validation, as the researchers find similar learning curves across a variety of test domains, &ldquo;although different applications yield different power-law exponents and intercepts&rdquo;. &nbsp;&nbsp;It is also a further sign that compute will become as strategic as data to AI, with researchers seeking to be able to run far more empirical tests and scale-up far more frequently when equipped with somewhat formal intuitions like the one stumbled upon by Baidu&rsquo;s research team.&ndash; Read more here: Deep Learning Scaling is Predictable, Empirically (Baidu blog).&ndash; Read more here: Deep Learning Scaling is Predictable, Empirically (Arxiv).
Evolution, evolution everywhere at Uber AI Labs:&hellip;Suite of new papers shows the many ways in which neuroevolution approaches are contemporary and complementary to neural network approaches&hellip;Uber&rsquo;s AI research team has published a set of papers that extend and augment neuroevolution approaches &ndash; continuing the long-standing professional fascinations of Uber researchers like Ken Stanley (inventor of NEAT and HyperNEAT, among others). Neuroevolution is interesting to contemporary AI researchers because it provides a method to use compute power to push simple algorithms through the more difficult parts of hard problems rather than having to invent new algorithmic pieces to get us across certain local minima; with evolutionary approaches, the difference between experimental success and failure is often dictated by the amount of compute applied to the problem.&ndash;&nbsp;&nbsp;Exploration: The researchers show how to further tune the exploration process in evolutionary strategies (ES) algorithms through the alternation of novelty search and quality diversity algorithms. They also introduce new ideas to improve the mutation process of large neural networks.&ndash;&nbsp;&nbsp;Theory: The researchers compare the approximate gradients computed by ES with the exact gradient computed by stochastic gradient descent (SGD) and design tools to better predict how ES performance relates to scale and parallelization.&ndash;&nbsp;&nbsp;Big compute everywhere: &ldquo;For neuroevolution researchers interested in moving towards deep networks there are several important considerations: first, these kinds of experiments require more computation than in the past; for the experiments in these new papers, we often used hundreds or even thousands of simultaneous CPUs per run. However, the hunger for more CPUs or GPUs should not be viewed as a liability; in the long run, the simplicity of scaling evolution to massively parallel computing centers means that neuroevolution is perhaps best poised to take advantage of the world that is coming,&rdquo; they write.&ndash; Read more here: Welcoming the Era of Deep Neuroevolution (Arxiv).&ndash; Read more: Deep Neuroevolution: Genetic Algorithms Are a Competitive Alternative for Training Deep Neural Networks for Reinforcement Learning (Arxiv).&ndash; Read more: Safe Mutations for Deep and Recurrent Neural Networks through Output Gradients.&ndash; Read more: On the Relationship Between the OpenAI Evolution Strategy and Stochastic Gradient Descent (Arxiv).&ndash; Read more: ES Is More Than Just a Traditional Finite Difference Approximator (Arxiv).&ndash; Read more: Improving Exploration in Evolution Strategies for Deep Reinforcement Learning via a Population of Novelty-Seeking Agents.
US National Security Strategy picks out AI&rsquo;s potential damage to the information battlespace:&hellip;AI&rsquo;s ability to create fake news and aid surveillance picked out in NSS report&hellip;While other countries around the world publish increasingly complicated, detailed national AI development strategies, the US government is …"

---

### Import AI: #74: Why Uber is betting on evolution, what Facebook and Baidu think about datacenter-scale AI computing, and why Tacotron 2 means speech will soon be spoofable

All hail the new &lsquo;datacenter scale&rsquo; era for AI:&hellip;Facebook Research Paper goes through some of the many problems that come with running AI at the scale of an entire datacenter&hellip;Facebook has published an analysis of how it runs its worldwide fleet of AI services and how its scale has influenced the way it has deployed AI into production. The company uses both CPUs and GPUs, with GPUs being used for large-scale face recognition, language translation, and the &lsquo;Lumos&rsquo; feature-analysis service. It also runs a significant amount of work on CPUs; one major workload is ranking features for newsfeed. &ldquo;Computer vision represents only a small fraction&rdquo; of the total work, Facebook writes.&nbsp;&nbsp;Split languages: Facebook uses &lsquo;Caffe2&rsquo; for its production systems, while its researchers predominantly use PyTorch. Though the company&rsquo;s main ML services (FBLearner Feature Store / FBLearner Flow / FBLearner Predictor) support a bunch of different AI frameworks, they&rsquo;ve all been specially integrated with Caffe2, the company says. &nbsp;&nbsp;The big get bigger: Facebook, like other major AI users, is experimenting with running significantly larger AI models at larger scales: this has altered how it places and networks together its GPU servers, as well as directed it to spin-up research in areas like low-precision training. They&rsquo;re also figuring out ways to use the scale to their advantage. &ldquo;Using certain hyperparameter settings, we can train our image classification models to very large mini-batches, scaling to 256+ GPUs,&rdquo; they write. &ldquo;For one of our larger workloads, data parallelism has been demonstrated to provide 4x the throughput using 5x the machine count (e.g., for a family of models that trains over 4 days, a pool of machines training 100 different models could now train 20 models per day, so training throughput drops by 20%, but the wait time for potential engineering advancement improves from four days to one day).&rdquo; &nbsp;&nbsp;One GPU region to train them all: When Facebook was first experimenting with GPUs for deep learning it rolled out GPUs in a single data center region, which it figured was a good decision as the designs of the servers were changing and the teams needed to become used to maintaining them. This Had some pretty negative consequences down the road, causing a re-think of how the company distributed its data center resources and its infrastructure.Read more: Applied Machine Learning at Facebook: A Datacenter Infrastructure Perspective.
Baidu publishes some rules-of-thumb for how model size relates to performance:&hellip;The beginnings of a theory for deep learning&hellip;Deep learning is an empirical science &ndash; we don&rsquo;t fully understand how various attributes of our neural networks dictate their ultimate representational capacity. That means the day-to-day work of any AI organization involves a lot of empirical experimentation. Now, researchers with Baidu have attempted to formalize some of their ideas about how the scale of a deep learning model relates to its performance. &nbsp;&nbsp;&ldquo;Through empirical testing, we find predictable accuracy scaling as long as we have enough data and compute power to train large models. These results hold for a broad spectrum of state-of-the-art models over four application domains: machine translation, language modeling, image classification, and speech recognition,&rdquo; they write.&nbsp; The results suggest that once researchers get a model to a certain threshold of accuracy they can be confident that by simply adding computer &amp;/or data they can reach x performance within a rough margin of error. &ldquo;Model error improves starting with &ldquo;best guessing&rdquo; and following the power-law curve down to &ldquo;irreducible error&rdquo;,&rdquo; they say. &ldquo;We find that models transition from a small training set region dominated by best guessing to a region dominated by power-law scaling. With sufficiently large training sets, models will saturate in a region dominated by irreducible error (e.g., Bayes error).&rdquo; &nbsp;&nbsp;The insight is useful but still requires experimental validation, as the researchers find similar learning curves across a variety of test domains, &ldquo;although different applications yield different power-law exponents and intercepts&rdquo;. &nbsp;&nbsp;It is also a further sign that compute will become as strategic as data to AI, with researchers seeking to be able to run far more empirical tests and scale-up far more frequently when equipped with somewhat formal intuitions like the one stumbled upon by Baidu&rsquo;s research team.&ndash; Read more here: Deep Learning Scaling is Predictable, Empirically (Baidu blog).&ndash; Read more here: Deep Learning Scaling is Predictable, Empirically (Arxiv).
Evolution, evolution everywhere at Uber AI Labs:&hellip;Suite of new papers shows the many ways in which neuroevolution approaches are contemporary and complementary to neural network approaches&hellip;Uber&rsquo;s AI research team has published a set of papers that extend and augment neuroevolution approaches &ndash; continuing the long-standing professional fascinations of Uber researchers like Ken Stanley (inventor of NEAT and HyperNEAT, among others). Neuroevolution is interesting to contemporary AI researchers because it provides a method to use compute power to push simple algorithms through the more difficult parts of hard problems rather than having to invent new algorithmic pieces to get us across certain local minima; with evolutionary approaches, the difference between experimental success and failure is often dictated by the amount of compute applied to the problem.&ndash;&nbsp;&nbsp;Exploration: The researchers show how to further tune the exploration process in evolutionary strategies (ES) algorithms through the alternation of novelty search and quality diversity algorithms. They also introduce new ideas to improve the mutation process of large neural networks.&ndash;&nbsp;&nbsp;Theory: The researchers compare the approximate gradients computed by ES with the exact gradient computed by stochastic gradient descent (SGD) and design tools to better predict how ES performance relates to scale and parallelization.&ndash;&nbsp;&nbsp;Big compute everywhere: &ldquo;For neuroevolution researchers interested in moving towards deep networks there are several important considerations: first, these kinds of experiments require more computation than in the past; for the experiments in these new papers, we often used hundreds or even thousands of simultaneous CPUs per run. However, the hunger for more CPUs or GPUs should not be viewed as a liability; in the long run, the simplicity of scaling evolution to massively parallel computing centers means that neuroevolution is perhaps best poised to take advantage of the world that is coming,&rdquo; they write.&ndash; Read more here: Welcoming the Era of Deep Neuroevolution (Arxiv).&ndash; Read more: Deep Neuroevolution: Genetic Algorithms Are a Competitive Alternative for Training Deep Neural Networks for Reinforcement Learning (Arxiv).&ndash; Read more: Safe Mutations for Deep and Recurrent Neural Networks through Output Gradients.&ndash; Read more: On the Relationship Between the OpenAI Evolution Strategy and Stochastic Gradient Descent (Arxiv).&ndash; Read more: ES Is More Than Just a Traditional Finite Difference Approximator (Arxiv).&ndash; Read more: Improving Exploration in Evolution Strategies for Deep Reinforcement Learning via a Population of Novelty-Seeking Agents.
US National Security Strategy picks out AI&rsquo;s potential damage to the information battlespace:&hellip;AI&rsquo;s ability to create fake news and aid surveillance picked out in NSS report&hellip;While other countries around the world publish increasingly complicated, detailed national AI development strategies, the US government is …