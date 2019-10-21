---
title: "Labeling Instruction Builder"
excerpt: ""
---
[block:api-header]
{
  "title": "What is a Labeling Instruction?"
}
[/block]
In order to give labeling task to freelance annotators, data science team needs to define specifications of a labeling task. Those specifications need to be converted to a user-experience. In TrainingData.io application specification builder is called labeling instruction. Labeling instruction is a list of objects that a data-scientist wants human-labelers to find in an image. Objects can have properties like color, size, shape etc. Data-scientist wants to present these properties in question-and-answer HTML form to the annotator.

Labeling instruction has two parts to it. Left panel and right panel. The left panel shows list of classes, their attributes and image-attributes. The right-panel shows how annotation-user-experience appear to the annotator (exactly). 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4413682-LabelingInstruction1.png",
        "LabelingInstruction1.png",
        1717,
        738,
        "#adb7b7"
      ],
      "caption": "Sample Labeling Instruction"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "How to create a new Labeling Instruction?"
}
[/block]
As you add a class or an attribute on left panel, you will observe same class and attributes will show up on the right panel in real time. 
[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fwww.youtube.com%2Fembed%2FZ1ZYpmFLaRc%3Ffeature%3Doembed&url=http%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DZ1ZYpmFLaRc&image=https%3A%2F%2Fi.ytimg.com%2Fvi%2FZ1ZYpmFLaRc%2Fhqdefault.jpg&key=f2aa6fc3595946d0afc3d76cbbd25dc3&type=text%2Fhtml&schema=youtube\" width=\"640\" height=\"480\" scrolling=\"no\" frameborder=\"0\" allow=\"autoplay; fullscreen\" allowfullscreen=\"true\"></iframe>",
  "url": "https://www.youtube.com/watch?v=Z1ZYpmFLaRc&feature=youtu.be",
  "title": "LabelingInterface Example",
  "favicon": "https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico",
  "image": "https://i.ytimg.com/vi/Z1ZYpmFLaRc/hqdefault.jpg"
}
[/block]

[block:api-header]
{
  "title": "Step 1: Creating First Class-Type"
}
[/block]
Classes are abstract-representation of real world objects that machine learning model learns about. Each class can have a:
1. Name: Associated real world object-class (like a car)
2. Color
3. Tool to be used to draw each object-instance belonging to that class
4. Sub-attributes are the properties of that class type
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/bea51e7-CarPolygon.png",
        "CarPolygon.png",
        495,
        243,
        "#f9fbfa"
      ],
      "caption": "New Class-type"
    }
  ]
}
[/block]

[block:html]
{
  "html": "<iframe width=\"560\" height=\"315\" src=\"https://www.youtube.com/embed/wc6oD7ZWCVo\" frameborder=\"0\" allow=\"accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture\" allowfullscreen></iframe>\n\n"
}
[/block]

[block:api-header]
{
  "title": "Step 2: Adding Attributes to Class-Type"
}
[/block]
Attributes define properties of real world objects. A simple example is color of car is a property of that car. Data scientists would want to know these properties, so that they can use it to train machines that make decision.  

An attribute is a question that you ask an annotator. There are four different data-types of an attribute:
1. Text: alphanumeric data entry
2. Multi-select Checkbox: a list of check boxes with multi-select functionality
3. Single-select Drop down list: with single select functionality
4. Single-select Radio button: with single selection functionality
[block:html]
{
  "html": "<iframe width=\"560\" height=\"315\" src=\"https://www.youtube.com/embed/3glJI8KxZng\" frameborder=\"0\" allow=\"accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture\" allowfullscreen></iframe>"
}
[/block]

[block:api-header]
{
  "title": "Step 3: Final Labeling Interface"
}
[/block]
After adding all classes and attributes to a labelling interface, a complete labelling interface will look like this:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/de94b8b-LabelingInterface.png",
        "LabelingInterface.png",
        1831,
        916,
        "#a9b6b5"
      ],
      "caption": "New Attribute"
    }
  ]
}
[/block]