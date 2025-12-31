# Identify the Car

Can a K-nearest neighbours classifier predict the make of a car from it's length, width, 
height, number of doors, and style?
This labtask has several parts:
- Collect the data for 10 cars.
  The sample must be a *Simple Random Sample*, and you must write a short explanation why your
  sample is a simple random sample.
  One smart idea is to head out to a random carpark on campus, Publix, etc., and sample the cars
  appropriately.
  Submit that justification in a file `SimpleRandomSample.pdf`. (0.5%)
- Put the data in an Excel spreadsheet called `MyCars.csv` with the columns `Length`, `Width`,
  `Height`, `Doors`, `Style`, and `Make`.
  The `Length`, `Width`, and `Height` are an integer number of inches.
  The `Doors` is an integer (count a hatchback as a door).
  The `Style` is one of `Sedan`, `SUV` (including Jeep Wranglers), `Pickup`.
  The `Make` is something like `Ford`, `Tesla`, `Nissan`, etc.
  You can get the data for a car by asking an LLM like ChatGPT (but feel free to walk around with
  a tape measure to get your data :-).
  Submit `MyCars.csv`. (0.5%)
- The TA will combine all the samples into one spreadsheet that everyone can use.
- Randomly split the data set into a training set of 80% and a testing set of 20%.
  Put the training set in a spreadsheet called `Training.csv` and the testing set in a spreadsheet
  called `Testing.csv`.
  Use K-nearest neighbours classification in Python to train the model, then predict the make of
  each car in the testing set.
  You must iterate over K to find the highest accuracy.
  Call the Python program `KNNClassifier.py`.
  Create a spreadsheet called `Accuracy.csv` with the columns `K` and `Accuracy`, and record the
  accuracy achieved for each `K`.
  Report the results for the `K` with the highest accuracy.
  Add three new columns to  `Testing.csv` called `Prediction`, and `Confidence` to store the
  prediction and confidence for each car in the testing set.
  Submit `Training.csv`, `Testing.csv`, `Accuracy.csv`, and `KNNClassifier.py`. (3.0%)
