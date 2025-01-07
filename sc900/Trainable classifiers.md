Trainable classifiers use [[Artificial Intelligence (AI)]] and [[Machine Learning (ML)]] to intelligently classify your data. They're most useful classifying data unique to an organization like specific kinds of contracts, invoices, or customer records. This method of classification is more about training a classifier to identify an item based on what the item is, not by elements that are in the item (pattern matching). Two types of classifier are available:
1. **Pre-trained classifiers** 
2. **Custom trainable classifiers** - Microsoft supports the ability to create and train custom classifiers. They're most useful when classifying data unique to an organization, like specific kinds of contracts, invoices, or customer records.
    

To get a custom trainable classifier to accurately identify an item as being in a particular category of content, it must first be presented with many samples of the type of content in the category. This feeding of positive samples is known as seeding and is used to create a prediction model for the classifier.

The model gets tested to determine if the classifier can correctly distinguish between items that match the category and items that don't. The result of each prediction is manually verified, which serves as input to improve the accuracy of the prediction model.

After the accuracy score of the model has stabilized, the classifier can be published. Trainable classifiers can then sort through items in locations like SharePoint Online, Exchange, and OneDrive, and classify the content.