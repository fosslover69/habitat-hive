# Habitat Hive

Habitat Hive is a project that's aimed to solve rental finding problems. Habitat Hive uses a Habitability Index which ranks properties based on the living well-being around the property.

## Problem 
Finding housing properties for rent these days is getting harder and harder. Think about livable housing, it's almost impossible to find.

## Solution  
Habitat Hive solves these problems using Machine Learning algorithms by giving habitability scores to every property listed. This makes the buyers make an easy and perfect decision.

## How we solved the problem?
The project utilizes a dataset obtained from Kaggle, comprising various features such as Property ID, Property type, property area, Number of windows, Number of doors, Furnishing, Frequency of Power cuts, Power backup, Water supply, traffic density score, crime rate, dust and noise, air quality index, neighbourhood review, and habitability score. As the habitability score prediction requires numerical values, all the discrete values were converted into numerical values (e.g., Furnished, Semi Furnished, and Unfurnished to 1, 0.5, and 0, respectively). 

To simplify the dataset, a new dataset was created only comprising common values such as property area, frequency of power cuts, power backup, water supply, traffic density score, crime rate, dust and noise, air quality index, and neighbourhood review for a particular area. This preprocessed dataset will be used for further prediction and model training.

## How do we present it?
There's no use in having a 100% perfect model that solves the problem in a split second if a normal end user can use it. So we created an Eye Candy Web App to present the model to the user. There's also a page on which you can calculate your own Habitability Index.

![image](https://user-images.githubusercontent.com/67329471/230719378-3d40e4a8-4dbb-42d6-aa31-1d8077758ee2.png)

## Technologies used
We used a wide range of technologies and we'd like to divide them into 3 parts

**Frontend:**
- [Svelte](https://kit.svelte.dev/) - The fun frontend framework of choice 
- [Flowbite](https://flowbite-svelte.com/) - Eye candy component library
- [TailwindCSS](https://tailwindcss.com/) - CSS from future

**Backend:**
- [Flask](https://flask.palletsprojects.com/en/2.2.x/) - Come on is there anything Python can't do?

**Machine Learning:**
- [Sklearn](https://scikit-learn.org/stable/index.html) - The Augur of the technology world
    - [DecisionTreeRegressor](https://spark.apache.org/docs/latest/api/python/reference/api/pyspark.ml.regression.DecisionTreeRegressor.html)
    - [AdaBoostRegressor](https://scikit-learn.org/stable/auto_examples/ensemble/plot_adaboost_regression.html)
- [OneAPI](https://www.oneapi.io/) - The Star of the Show

## Why we chose OneAPI?
OneAPI is a powerful tool for machine learning projects that can help developers achieve better performance and code portability. With its optimized libraries, performance tools, and unified programming model, OneAPI can speed up training and improve inference performance, while simplifying development by enabling developers to write code that can run on different hardware platforms.

Its key benefits include:

- Accelerating training on hardware accelerators, such as GPUs or FPGAs
- Improving inference performance on various hardware platforms, which can reduce latency and improve throughput
- Increasing code portability by enabling developers to write code that can run on different hardware architectures
- Optimizing performance with performance tools that can help developers improve the performance of their code
- Simplifying development with a unified programming model that can help reduce the need for platform-specific code.

### Benchmarks
Using oneAPI in our project provided us with around 2% uplift in accuracy. This may seem like a tiny improvement but on larger datasets this will impact accuracy on a larger scale.

Our Benchmarks:

![image](https://user-images.githubusercontent.com/67329471/230724347-783ff7fc-969e-4999-9e80-b37e970fd3b1.png)

Convinced with the performance of oneAPI? To integrate it with your project: [click here!](https://github.com/fosslover69/habitat-hive/blob/main/oneAPI-Integration.md)

## User Guide:

English:


https://user-images.githubusercontent.com/67329471/230719124-d3511eff-04b1-4487-b2a8-f2587efb2a8a.mp4




Tamil:


https://user-images.githubusercontent.com/67329471/230719128-9a730d3e-8c55-418e-9aa7-4cd7a16b49e5.mp4



