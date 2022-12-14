# Assignment-4


Testing machine learning projects is challenging and there is no one standard way of doing it. Due to the fact that ML projects are heavily dependent on data and models that cannot be strongly specified as learnig  network, testing ML projects is a more complex challenge than testing traditional softwares. In contrast to most conventional software tests, ML project tests have to include data tests, model tests, as well as tests in production.
First of all, ML projects have a lot more uncertainty than traditional software. In many cases, we don’t know if the project is even technically possible and what will be results (like a result can be in a range), so we have to give some time to conduct research and give an answer for this problem as well. This uncertainty harms good software practices such as testing because we don’t want to spend time on testing ML projects in an early stage of development, which might not receive the GO signal for further continuation.
On the other hand, the more the project stays without testing, the more technical complexities it creates for future testing. As the ML project matures, we have to start focusing more and more on increasing testing coverage.



In contrast to conventional software testing, in ML testing we need to pay special attention to data testing. ML systems differ from traditional software-based systems in that the behavior of ML systems is not specified directly in code but is learned from data. If the input data has some defects then we can’t expect that the ML model will produce optimal results. 
Lastly, it’s crucial to make sure that the ML system works correctly not only in development and launch but that it continues to work correctly in production as well. In traditional software, tests are only run in the development environment and it’s assumed that if a piece of code reaches production, it must have been tested and works properly. Over time in ML projects, some external conditions might cause data shifts or we might change the data source and provider. That’s why we need to continue testing and monitoring the ML system using output logs.



As we explained above, testing ML projects is way more complicated than testing conventional software. Besides that, there are a lot of things that we need to pay attention to. Especially since some of them are happening downstream in the ML system pipeline. For instance, anomalies in the prediction might not be because of the model but because of the input data.



Some of the critical issues in an ML project are:



Data issues: Missing values, data distribution shift, setup problems, the impossibility of reproducing input data, inefficient data architecture, etc.
Model issues: Low model quality, large model, different package versions, etc.
Deployment issues: unstable environment, broken code, training-serving skew, etc.



However we can use a few handy tools to test ML models



For unit testing, the default unit testing framework in Python is Unittest. It supports test automation, sharing of setup and shutdown code for tests, aggregation of tests into collections, and independence of the tests from the reporting framework.



Also, Unittest has unittest.mock module that enables using mock objects to replace parts of the ML system under test and make assertions about how they were used. For that, it provides a Mock class that intends to replace the use of test doubles throughout the project. Mocks keep track of how we use them, allowing us to make assertions about what code has done to them. 



Another library intended to help write unit tests for applications is Pytest. Pytest is built on 3 main concepts that include test functions, assertions, and test setup. It has a naming convention for writing tests which allow automatically running tests.



Also, Deepchecks is a Python package for comprehensively validating your machine learning models and data with minimal effort. This includes checks related to various types of issues, such as model performance, data integrity, distribution mismatches, and more.



Concluding these findings we can say that it feels a little tricky in the start about testing our machine learning models and especially with automation. However, different tools are available which have matured now to provide us a good experience in automation
