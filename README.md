Download Link: https://assignmentchef.com/product/solved-ct5133-ct5145-assignment-2a
<br>
Transfer Learning, Convolutions, and Object Localisation in Keras




<ul>

 <li><strong>Weight</strong>: 20% of the module</li>

 <li><strong>Deadline</strong>: Midnight Sunday 2nd May, end of Week 11.</li>

 <li><strong>Teams</strong>: You may work solo, or in a group of 2. The assignment is the same either way. If working in a group of 2, you may not work with a student with whom you have worked in any previous assignment in this module or any other module.</li>

</ul>

<ol>

 <li>Create a labelled image classification dataset, OR choose an existing one. It should include <strong>exactly 2 classes</strong>. The classification problem should be suitable for deep convolutional networks, e.g. not trivially solved with colour thresholding. If you like, you can choose just two classes from an existing dataset. If using an existing dataset, do not use MNIST, Fashion MNIST, CIFAR, ImageNet, or any subset of them. <strong>Update</strong>: do not use a dataset created for any previous module, such as the SUV versus Sedan car dataset. Write a short paragraph to describe the dataset: background, size/shape, classes, method of collection. Include a typical image from each class.</li>

 <li>Choose any pretrained image classification model, e.g. one of those found at <a href="https://keras.io/api/applications/">https://keras.io/api/a </a><a href="https://keras.io/api/applications/">pplications/.</a> Import it, excluding the dense classification head. Make sure to use the appropriate preprocessing for input images. We will call this the base model. Add layers to the base model and train them to produce classifications on your dataset. Report your choice of base model; state and explain the shape of the base model’s output; explain the layers you added and training carried out; report classification performance on unseen data.</li>

 <li>Now investigate the base model as follows. Extract a scalar output from each neuron in the final layer of the base model. You can use a GlobalMaxPooling2D layer or GlobalAveragePooling2D, or another method if you prefer. Add a Softmax layer after. Using this, <strong>identify one or more neurons whose scalar output is strongly correlated with the class label of your dataset. </strong>Such neurons can be seen as (weak) class detectors. Specify your method, state results, and give brief interpretation of the results.</li>

 <li>Now build a simple approach to object localisation, that is deciding <strong>where </strong>in the input image an object is present, as follows. For each neuron identified in (3), write code to <strong>visualise its 2D output</strong>. Use this to write a brief comment: <strong>does this 2D output allow localisation of objects in the input image? </strong>Include several example images and the corresponding 2D outputs to support your comment. Note: if we fail to make step (3) work, step (4) can still be attempted by choosing some neurons manually. By the way, this approach is related to but not very similar to state of the art systems for object localisation, such as YOLO. We are not required to investigate such systems in this assignment.</li>

</ol>

<ul>

 <li><strong>Submission</strong>: Submit <strong>either </strong>a .ipynb file, or a .pdf and a single .py file. Include student name(s) and ID(s) at the top of every file submitted. The report and code should be in four sections corresponding to points 1-4 above. Code should be well structured and commented. Include a citation and/or URL for any sources used, such as code, papers, and blogs. Do not submit the dataset, but include a link, source, or download instructions if available. Marks will be deducted for incorrect submission formats.</li>

 <li><strong>Plagiarism</strong>: NUI Galway guidelines on plagiarism apply. You may discuss the assignment with other students/groups but may not view any part of their solution or allow them to view yours.</li>

</ul>