# Deep Learning Model Generation

1. TOC
{:toc}

During the past few weeks, I have learnt how models can be generated using deep learning techniques, and even made my own using the CIFAR10 dataset. 

## Downloading using DuckDuckGo

The duckduckgo_search package was effective in being able to scrape the web for a lot of images. However, I did note that this procedure was time consuming, and trying to collect 200 images each for 10 different classes took me 22 minutes to complete.

{% include info.html text="Web Scrabing is effective, but can be time consuming" %}

## Image Classification

I used the below functionality to perform image classification

Python code and output:

```python
entropy = CrossEntropyLossFlat()
learn = vision_learner(dls, resnet18, metrics=accuracy, loss_func = entropy)
learn.fine_tune(3)
```

I found loss functions were useful in multi-class learning models, such as the CIFAR10 model.

## t-SNE plots


T-SNE plots are like a secret decoder for high-dimensional data, unlocking hidden patterns and structures with stunning visual clarity. Here's why they're so cool:

- Dimensionality Reduction Magic: T-SNE (t-Distributed Stochastic Neighbor Embedding) works like a magician's sleight of hand, reducing complex, multi-dimensional data into a 2D or 3D plot without losing too much information. It's like compressing a large file into a manageable size without sacrificing quality.
- Visual Poetry: T-SNE plots transform abstract numbers into visual poetry. They unveil the underlying relationships between data points in a way that's visually intuitive and aesthetically pleasing. Clusters emerge like constellations in the night sky, each telling its own unique story.
- Cluster Visualization: Ever wondered how similar or dissimilar your data points really are? T-SNE reveals clusters of points that share common traits or features. Whether it's grouping similar images in a dataset or identifying distinct customer segments, T-SNE makes it easy to spot patterns and outliers.

## Confusion Matrices

Confusion matrices seem to do the opposite of confuse me. They helped me identify if my learning model was performing accurately. An example confusion matrix can be found [here](https://images.datacamp.com/image/upload/v1701364260/image_5baaeac4c0.png).







