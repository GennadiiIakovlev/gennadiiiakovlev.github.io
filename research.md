---
title: "Ongoing Research"
permalink: /research/
layout: single
---



**Authoritarian resource distribution to civil society and political legitimation in Russia**

*[preprint is here](https://osf.io/preprints/socarxiv/q25nf_v2)*

*together with [Francesca Chiarvesio] (https://scholar.google.com/citations?user=bCkYwusAAAAJ&hl=ru) -- postdoctoral fellow at the University of Bern*

Authoritarian resource distribution to civil society andpolitical legitimation in RussiaFrancesca Chiarvesio and Gennadii IakovlevAbstractHow do authoritarian legitimation strategies shape the allocation of state resourcesto civil society organizations, and what kind of alignment between state and civil soci-ety’s action do they produce? This article addresses these questions by analyzing Rus-sia’s Presidential Grants. By operationalizing the regime’s ideology and performance-based legitimation strategies through state grant redistribution, this work reveals ameta-regulated, state-engineered non-profit sector. The government reshapes civil so-ciety’s behavior primarily through centralized rules and standards rather than corpo-ratism and co-option. In addition, the findings challenge the expectation that performance-based legitimation strategies straightforwardly produce depoliticization and highlightthe underexamined role of technocratic governance in sustaining authoritarian resilience.The analysis is based on computational text analysis of over 150,000 grant applicationssubmitted by civil society for project funding between 2017 and the first half of 2025.
![This graph shows the factors responsible for the receptance and non-receptance of grants](/assets/presi_ame.png)

This graph shows which target age (calculated from application content using aritificial intelligence) is more exposed to state ideology. Those are not yong children, but teenagers and students that are mostly exposed.
![This graph shows which target age (calculated from application content using aritificial intelligence) is more exposed to state ideology. Those are not yong children, but teenagers and students that are mostly exposed.](/assets/targ_age_to_target_audience.png)


**Stylometry Meets Transformer Embeddings**

*together with [Levente Littvay](https://levente.littvay.hu) -- my mentor since my move to Budapest.*

Political speeches, tweets, and press releases often come from a team of ghost‑writers. Stylometry—the science of measuring writing style —has long tried to unmask real authors, but the field is being revolutionized by large language models (LLMs). Can off‑the‑shelf embeddings of state-of-the art transformer LLMs sharpen our ability to assign (or dispute) authorship?

The first approach sticks to classics that any computational social science scholar can already run: sentiment dictionaries, TF–IDF with truncated SVD, and t-SNE plots. The second feeds exactly the same texts through progressively larger language-model encoders: domain-tuned BERT variants for English tweets, a nimble 7-billion-parameter Qwen that will run on a consumer GPU or an Apple-Silicon laptop, and a 72-billion-parameter edition that shows what “best possible” separation looks like. For every text we clusterize the embeddings into 2 or 3 groups, drop them into UMAP (Uniform Manifold Approximation and Projection, a learning technique for dimension reduction that came after t-SNE), and let k-means decide where the writing styles part company.

We validate the method on two ground-truth tasks: 3,800 Donald Trump’s Android-vs-iPhone tweets and 24 scripted-vs-impromptu speeches. While the two approaches both spot the authorial fingerprint, the embeddings draw cleaner, much more separated clusters, especially when the case gets more complicated.  On a smaller number of much longer speeches, those dictionary counts collapse into noise, but even the mid-sized encoder keeps the scripted and improvised talks in largely distinct UMAP islands.

The purple island on the right is dominated by iPhone tweets, while the green island on the left is almost entirely Android. Embeddings separate devices more crisply, as opposed to dictionary features.
![](/assets/qwen72b_tweets_3cl_100dim.png)
*Figure 1. UMAP projection of tweet embeddings (Qwen 2.5 72B) clustered into three groups. Points are coloured by k‑means cluster (green = Cluster 1, orange = Cluster 2, purple = Cluster 3) and shaped by device (● Android, + iPhone).*

![](/assets/UMAP Projection by Teleprompter Usage Roberta.png)
*Figure 2. UMAP projection of speech embeddings (Roberta) clustered into two groups. Points are coloured by the usage of teleprompter (blue = Not Used, orange = Used).*

We then plan to apply our approach on 1000 Hungarian speeches by Viktor Orbán, where true authorship is unknown. By contrasting classic stylometry with progressively larger LLM encoders, we hope to see  the speech writers.

**Do Terrorist Attacks Shift Parliamentary Rhetoric? Evidence from Germany**
**Preliminary findings from an LLM assisted analysis** 

*together with [Gustavo Venturelli](https://venturelligustavo.com) -- Assistant Professor at the Stetson University*

Conventional wisdom suggests that dramatic acts of violence, such is terrorism, push politicians toward tougher, often anti-immigration, positions. Yet systematic evidence for such rhetorical shifts remains thin. We set out to test the hypothesis in the German Bundestag: Do members of parliament (MPs) become more negative toward immigrants in the immediate aftermath of terrorist attacks?

We used the corpus of roughly 250,000 speeches delivered in the Bundestag between 2014 and 2024. First, we analyzed every parliamentary speech using Large Language Models (LLMs). A lightweight LLM first marked any speech that mentioned migration. ChatGPT 4o was then used to distinguish between the evaluation of how the state handles migration policies and an emotion towards migrants per se. To isolate causal effects we ran a regression discontinuity in time design around four widely covered attacks between 2015 2019, using a ±30 day window atfer each event.

No statistically meaningful jump appears in either series. The figure below plots weekly averages with 95 % confidence bands; tone before and after each attack overlaps.

*Figure: Weekly average emotional tone of Bundestag speeches that discuss migration policy (gold) and migrants themselves (orange). Shaded bands represent 9 % confidence intervals; vertical red dashed lines mark each terror attack. The grey rectangle shows the 2016 summer recess, illustrating how parliamentary holidays interrupt the time series.*
![](/assets/ter-rdd.jpeg)

In Germany, at least, parliamentary rhetoric on migration seems insulated from short term security shocks. Hovewer, one of our for attacks happened during the parliamentary holidays, and the other two in the neighbouring countries. The absence of effect can be caused by insifficient data. 

If confirmed, the finding complicates the common narrative that terrorism automatically hardens elite attitudes toward immigrants. Instead, rhetorical responses may depend on parliamentary calendars, media framing, and the geography of violence. For scholars, the project showcases how off the shelf LLMs can open new frontiers in the systematic study of political speech.





