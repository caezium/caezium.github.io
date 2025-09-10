---
title: "Understanding Statistical Data Types"
source: "https://towardsdatascience.com/understanding-statistical-data-types-2993dafcac86/"
author:
  - "[[Rohan Vij]]"
published: 2022-07-22
created: 2025-06-20
description: "\"Data is the new oil\" - but just like several types of oil exist, so do several types of data."
tags:
  - "clippings"
---
## Summary
The article \\"Understanding Statistical Data Types\\" introduces fundamental data classifications, starting with qualitative (categorical) and quantitative (numerical) data. It then details four main subtypes: nominal and ordinal data under qualitative, and discrete and continuous data under quantitative. For each type, it provides definitions, characteristics, and examples, explaining their differences in terms of measurement, order, and mathematical applicability.

## Key Points
- Data is crucial and knowing its types is essential for operation.
- **Qualitative (Categorical) Data:** Cannot be numerically measured; grouped into categories (e.g., sex, race).
    - **Nominal Data:** Distinct labels without inherent order (e.g., eye color).
    - **Ordinal Data:** Variables have a natural order or ranking, indicating relative differences (e.g., education level).
- **Quantitative (Numerical) Data:** Quantifiable and usable in mathematical analyses (e.g., time, weight).
    - **Discrete Data:** Involves whole numbers, countable but not measurable (e.g., number of people).
    - **Continuous Data:** Involves fractions, measurable but not countable (e.g., time, height).
- These four data types form the backbone of statistical data types.

---

https://towardsdatascience.com/understanding-statistical-data-types-2993dafcac86/
# Original Content

![Photo by Markus Spiske on Unsplash](https://towardsdatascience.com/wp-content/uploads/2022/07/0TkQNQJ064GlU9Yf--scaled.jpg)

Photo by Markus Spiske on Unsplash

## Introduction

"Data is the new oil" – a phrase coined in 2006 which took the world by storm.

Wants some [shocking facts](https://cloudnine.com/ediscoverydaily/electronic-discovery/date-fun-facts-big-data-ediscovery-trends/)? Over 90% of all data in the world was created in the last two years. If you burned all the data generated in a day onto CDs, that stack could reach the mean twice. Data is big and valuable – so knowing how to operate on it is crucial. To do so, it is crucial to learn about the different types of data and what they represent. Let’s get started!

## Qualitative vs Quantitative

Now, you have probably gone over this several times throughout your life, so I will keep this short. Qualitative data (also known as categorical data) is data that cannot be measured using numbers. When sorting categorical data, one can only group them into categories. Common examples of categorical data are sex (male/female), race, and educational level.

Quantitative data is exactly what you might guess – quantifiable (numerical) data. Quantitative data can be sorted (think greatest to lowest), graphed, and used in mathematical analyses. Some common examples of quantitative data are time, weight, temperature, and grade level.

We can treat these two types of data, qualitative and quantitative data, as the root of the other four data types we will be exploring.

## Types of Qualitative Data

### Nominal Data

Nominal data is a type of categorical data in which each data variable cannot be compared to one another. While each variable is different from the other, they are not relatively different from each other. For instance, eye color is an example of nominal data. While several types of eye color exist (black, brown, green, blue), we cannot say that they are different in relation to each other – they are simply labels describing an attribute. The meaning of the aforementioned list of eye colors would not change if we were to change its order.

### Ordinal Data

Ordinal data is data where each data variable is naturally related to the other. Each one is relatively different from the other, whether it be in terms of size, length, duration, etc. For example, education level (in this case college degrees) is a type of ordinal data. We can say that associate, bachelor’s, master’s, and doctoral degrees are all relatively different from one another because each requires a different about of time. Theoretically, we could quantify ordinal data (associate=2 years, bachelor’s=4 years, etc) and perform mathematical operations on it, so it is sometimes considered to be in a gray area between qualitative and quantitative data.

While ordinal data is also simply labels, the background information behind the labels can be compared to each other. As a result, if we were to reverse the order of the aforementioned list of college degrees, its order would change from least time → most time to most time → least time.

## Types of Quantitative Data

### Discrete Data

You have probably heard about discrete data during your middle and high school math classes. Chances are, you visualize discrete data through a graph like this:

![Image by the author.](https://towardsdatascience.com/wp-content/uploads/2022/07/1JRz-aD0rbkiLwyvx0M8dag.png)

Image by the author.

Data that only involves integers that are discrete (or separate) from one another. For example, the number of people in a room is an example of discrete data. It can only be measured in whole numbers – after all, you cannot have a fraction of a person! Discrete values can be counted because there is an exact set of them, but they cannot be measured.

### Continuous Data

Continuous data is data that involves fractions, or non-whole numbers. You most likely visualize it through a line:

![Image by the author.](https://towardsdatascience.com/wp-content/uploads/2022/07/1JzuOSoXpclhH675lndabbg.png)

Image by the author.

Continuous data consists of values such as time, height, and the price of an item. Each value can get divided or become smaller and still remain valid. For example, we can divide the time a person took to complete a race by two and it still will remain valid – even if the number goes into milliseconds and microseconds. On the other hand, we cannot always divide the number of people in a room by two. Again, you cannot have a fraction of a person! You can *measure* any continuous value, but you cannot *count* it (there are infinitely many points to count).

## Conclusion

![Image by the author.](https://towardsdatascience.com/wp-content/uploads/2022/07/1KkyNLz3FCFGYe2etvTWIgA.png)

Image by the author.

While these 4 data types mentioned in this article do form the backbone of statistical data types, several more subtypes exist under the ones already mentioned. If you want to read more, I highly recommend [this article by Niklas Donges](https://towardsdatascience.com/data-types-in-statistics-347e152e8bee) which goes more into depth.

---

Thank you for reading! I hope you thoroughly enjoyed the article and now are more comfortable with statistical data types.

---

Topics:

## Related Articles

- ![](https://towardsdatascience.com/wp-content/uploads/2024/08/0c09RmbCCpfjAbSMq.png)
	Step-by-step code guide to building a Convolutional Neural Network
- ![Photo by Krista Mangulsone on Unsplash](https://towardsdatascience.com/wp-content/uploads/2024/08/0GyVVTbgotH-DhGPH-scaled.jpg)
	Photo by Krista Mangulsone on Unsplash
	A beginner’s guide to forecast reconciliation
- ![Photo by davisuko on Unsplash](https://towardsdatascience.com/wp-content/uploads/2024/08/1bAABgtZtAIG5YW1oEjW3pA-scaled.jpeg)
	Photo by davisuko on Unsplash
	Here’s how to use Autoencoders to detect signals with anomalies in a few lines of…
- ![Image from Canva.](https://towardsdatascience.com/wp-content/uploads/2024/08/1UAA9jQVdqMXnwzYiz8Q53Q.png)
	Image from Canva.
	Feature engineering, structuring unstructured data, and lead scoring
- Solving the resource constrained project scheduling problem (RCPSP) with D-Wave’s hybrid constrained quadratic model (CQM)
- ![](https://towardsdatascience.com/wp-content/uploads/2023/02/1VEUgT5T4absnTqBMOEuNig.png)
	An illustrated guide on essential machine learning concepts
- ![](https://towardsdatascience.com/wp-content/uploads/2024/08/1kM8tfYcdaoccB1HX71YDig.png)
	Derivation and practical examples of this powerful concept