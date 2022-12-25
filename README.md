# New-particle-formation-event
The term project is on a data set about new particle formation (NPF). NPF happens on some days when small particles (starting from individual molecules) begin to form larger new particles. The particles then spread out of the forest and affect cloud formation and weather. In urban environments, air pollution is often caused by larger particles forming from anthropogenic sources, such as car exhausts, with dire consequences for human health. An interesting research question is under what conditions NPF happens, which is what your classifier will try to model. The NPF formation process is one of the significant scientific outputs from the University of Helsinki in atmospheric sciences. You can find a detailed explanation of the NPF phenomenon from Kerminen et al. (2018).

The training data file npf_train.csv contains several variables measured on different days (rows of the file) at the Hyytiälä forestry field station (mainly at the SMEAR II mast, shown in the picture). The variables are daily means and standard deviations of various measurements between sunrise and sunset. The variable names typically refer to the height of the measurement device in the mast. For example, T48 refers to the temperature at 4.8 meters above the mast base and T672 at 67.2 meters above the mast base (as you can see, the mast is quite tall). CS is the condensation sink in units of 1/s; for details, see Kulmala et al. (2012). You can find more details about the variables at https://smear.avaa.csc.fi/ or via https://wiki.helsinki.fi/x/XYiKDg.
On each day, an NPF event can occur. The type of NPF event is given in column “class4”: nonevent means no NPF event took place, and Ia, Ib, and II are different NPF event types. For the event classification schema and explanation of event types, see Dal Maso et al. (2005). For more information about the classification task, see Hyvönen et al. (2005) or Joutsensaari et al. (2018).
An in-depth understanding of the datasets or articles mentioned above is optional for completing the task (from a machine learning viewpoint, this is a relatively standard classification task!). However, understanding your modelling processes allows you to build better models and sanity-check the results.
The data files are pretty “clean” (e.g., no missing values), so you can hopefully concentrate on the machine learning part instead of fighting with the data.

# Your task

You should work in groups of 1-3 students.
Your task is to build and apply a classifier to predict the event types for days listed in the test data file npf_test_hidden.csv. The “primary” task is to make a binary classifier (event vs nonevent) for a new variable “class2”, defined as follows: “class2” = nonevent if “class4” is nonevent and “class2” = event if “class4” is one of Ia, Ib, or II. You don’t need to, and usually should not, code your classifier from scratch! You should use various machine learning libraries as in ”real life”.
Remember that this is a non-trivial classification task. It is possible to do it in many ways. The most straightforward binary classification task, classifying events vs. nonevents, is possible with reasonable accuracy using any decent machine learning library with little effort. Multi-label classification is more complex but should still be doable. However, you should also do the data exploration, preprocessing, feature selection, model selection, classification accuracy estimation etc., appropriately since you will report and analyse your choices and results in the project deliverable.
The project’s purpose is not to (even try to!) replicate any methods in the literature, make a super-complex best-performing classifier that beats everything else or attempt to use other data sources etc., to obtain the best possible classification accuracy. Do not use any method that you do not understand yourself! Accuracy of the predictions on the test data is not a grading criterion by itself, even though a terrible accuracy may indicate something else fishy in your approach (which could affect grading).

# My work

**1.Data Cleaning and Feature selection.**

**2.Normalisation**

**3.Built Machine Learning Models**

**4.EDA**

**5.Model Selection**
