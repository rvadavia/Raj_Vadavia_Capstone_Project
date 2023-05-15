>   **Abstract:**

>   As we approach the submission of the capstone project, which reflects my culmination of learning and understanding in ML, I have realized that there is still much more to learn to effectively apply it in a real-world context.

>   For instance, I am developing the initial Pay-Per-Use dermatology Electronic Medical Record (EMR) solution tailored to the Indian market. A valuable feature that would greatly benefit doctors is a patient complaint triage system. However, our platform, symabMED.in, is not yet prepared for implementation. Our system must run continuously for 12 to 18 months to gather relevant metadata and high-resolution images with accurate categorization for a real-world scenario in India. This data collection phase is crucial to ensure the effectiveness and reliability of our solution.

![A screenshot of a computer Description automatically generated with medium confidence](media/08a7bc76cabdf26c35148bb6281cfc58.png)

>   In the meantime, developing a generic framework using the HAM10000 dataset in the interim would be beneficial. This dataset can be a valuable resource for training and initial system testing. Furthermore, by building and fine-tuning the framework with this dataset, you can assess its performance, make necessary improvements, and gain valuable insights before incorporating the actual data from the Indian market.

>   Skin cancers encompass a range of diseases marked by the presence of abnormal growths or persistent sores that do not heal, as well as alterations in the size, shape, or colour of moles. There are two primary types: melanoma (less prevalent but more hazardous) and non-melanoma skin cancers (more common but less severe).

>   Notably, India experiences a relatively lower incidence of skin cancer than Western countries. This can be attributed, in part, to individuals with darker skin being less susceptible to this condition. The higher levels of melanin in darker skin provide a certain degree of protection against damage caused by UV radiation, thereby reducing the risk of developing skin cancer

>   However, regional variations can play a role in the prevalence of skin cancer in India: our system, in addition to other standard data like age, gender and what is included in the HAM dataset, a new training data may include the following features.

>   Latitude: Regions closer to the equator receive more intense sunlight, increasing the risk of skin cancer. Hence, regions in the southern part of India may see a slightly higher incidence rate.

>   Altitude: Higher altitudes receive more UV radiation. Therefore, areas at higher elevations could potentially have a higher incidence of skin cancer.

>   Outdoor occupations: In regions where more people work outdoors (like farming communities), there are increased sun exposure and a potentially higher risk of skin cancer.

>   Urban vs rural: Urban areas might see different rates due to lifestyle differences, including more indoor work and potentially more access to healthcare for early detection.

>   Cultural and social practices: Clothing, sunscreens, and shade can vary by region and influence skin cancer rates. Some traditional attire covers much of the body, providing natural sun protection

>   I intend to build a generic framework as part of my capstone project. This framework consists of the following routines by taking in DataFrame.

-   Pre and post-reports to provide details of the dataset
-   feature cleaning and normalization (such as one-hot encoding and replacing null values)
-   standardize the image files and remove corrupt images
-   identify a suitable machine-learning model for categorization prediction.

>   By developing and implementing these routines, I aim to enhance the quality and consistency of the metadata within the dataset, ensuring that it is well-organized and suitable for further analysis, ensuring that the dataset remains reliable and accurate for subsequent image-based analysis and processing.

>   I intend to test this routine using the HAM10000 dataset from the year 2020.

>   If all components of the project work as intended, you will have a comprehensive codebase capable of handling any DataFrame for image classification. Furthermore, the framework will facilitate data visualization and preparation for ML modelling, including selecting appropriate models. Additionally, I aim to provide an API that can be utilized as a real-world service.

>   **Problem Statement**:

>   "Develop a machine learning model to assist dermatologists in India with triaging skin conditions. The model should classify different skin conditions based on images, aiding in quicker and more efficient preliminary diagnosis. The target is to improve the efficiency of dermatologists by reducing their workload, enabling them to focus on more complex and urgent cases. The model is not intended to replace human diagnosis but to supplement it, serving as a first-line screening tool."

-   Step 1: define a variable for the row CSV file
-   Step 2: write a code for pre-processing the dataset
    -   Create DataFrame
    -   Sumerzies the datset inormation
    -   Visualize the data set
    -   Report the issues
-   Step 3: write a code for processing the dataset
    -   feature cleaning and normalization (such as one-hot encoding and replacing null values)
    -   standardize the image files and remove corrupt images
    -   Balance the data in the dataset
    -   Write a new CSV file and images files
-   Step 4: write a code for Post-processing the dataset
    -   Create DataFrame from the new CSV file
    -   Sumerzies the datset inormation
    -   Visualize the data set
    -   Create Train and Test data set
-   Step 5: write a code to identify a suitable machine-learning model
    -   Compare machine-learning model using Train and Test dataset
    -   Visualize the result
-   Step 6: write an API to execute the model for prediction

\-------------------- draft visualization and data cleaning

![A picture containing text, screenshot, rectangle, diagram Description automatically generated](media/bc9b965297fb58eead630074d80653c6.png)

![A picture containing text, diagram, screenshot, plot Description automatically generated](media/371c722cd098bce3123235a6be03090d.png)

![A picture containing text, screenshot, diagram, plot Description automatically generated](media/57e47f9d642cc22f57be8a2883589007.png)

![A picture containing text, screenshot, display, software Description automatically generated](media/aab62ee876e312b5facd35d41a435573.png)

>   Recommendations:

>   \- Column 'image_name' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'patient_id' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'sex' has missing values. Consider using dropna() or fillna().

>   \- Column 'sex' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'age_approx' has missing values. Consider using dropna() or fillna().

>   \- Column 'age_approx' is numerical. Consider scaling it using standard scaling or min-max scaling.

>   \- Column 'anatom_site_general_challenge' has missing values. Consider using dropna() or fillna().

>   \- Column 'anatom_site_general_challenge' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'diagnosis' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'benign_malignant' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'target' is numerical. Consider scaling it using standard scaling or min-max scaling.

>   Recommendations - END -:

>   Recommendations:

>   \- Column 'image_name' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'patient_id' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'sex' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'age_approx' is numerical. Consider scaling it using standard scaling or min-max scaling.

>   \- Column 'anatom_site_general_challenge' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'diagnosis' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'benign_malignant' is categorical. Consider encoding it using label encoding or one-hot encoding.

>   \- Column 'target' is numerical. Consider scaling it using standard scaling or min-max scaling.

>   Recommendations - END -:

>   DataFrame 1 info:

>   \| index \| Name \| Count \| Non-Null \| Dtype \|

>   \|--------:\|:------------------------------\|--------:\|:-----------\|:--------\|

>   \| 0 \| image_name \| 33126 \| non-null \| object \|

>   \| 1 \| patient_id \| 33126 \| non-null \| object \|

>   \| 2 \| sex \| 33061 \| non-null \| object \|

>   \| 3 \| age_approx \| 33058 \| non-null \| float64 \|

>   \| 4 \| anatom_site_general_challenge \| 32599 \| non-null \| object \|

>   \| 5 \| diagnosis \| 33126 \| non-null \| object \|

>   \| 6 \| benign_malignant \| 33126 \| non-null \| object \|

>   \| 7 \| target \| 33126 \| non-null \| int64 \|

>   :

>   DataFrame 2 info:

>   \| index \| Name \| Count \| Non-Null \| Dtype \|

>   \|--------:\|:------------------------------\|--------:\|:-----------\|:--------\|

>   \| 0 \| image_name \| 33126 \| non-null \| object \|

>   \| 1 \| patient_id \| 33126 \| non-null \| object \|

>   \| 2 \| sex \| 33126 \| non-null \| object \|

>   \| 3 \| age_approx \| 33126 \| non-null \| float64 \|

>   \| 4 \| anatom_site_general_challenge \| 33126 \| non-null \| object \|

>   \| 5 \| diagnosis \| 33126 \| non-null \| object \|

>   \| 6 \| benign_malignant \| 33126 \| non-null \| object \|

>   \| 7 \| target \| 33126 \| non-null \| int64 \|

>   :

>   Missing values in df1 :

>   image_name 0

>   patient_id 0

>   sex 65

>   age_approx 68

>   anatom_site_general_challenge 527

>   diagnosis 0

>   benign_malignant 0

>   target 0

>   Missing values in df2 :

>   image_name 0

>   patient_id 0

>   sex 0

>   age_approx 0

>   anatom_site_general_challenge 0

>   diagnosis 0

>   benign_malignant 0

>   target 0

>   :

>   Unique values df1 - df2:

>   image_name: 33126 --- 33126

>   patient_id: 2056 --- 2056

>   sex: 2 --- 2

>   age_approx: 18 --- 20

>   anatom_site_general_challenge: 6 --- 6

>   diagnosis: 9 --- 9

>   benign_malignant: 2 --- 2

>   target: 2 --- 2

>   sex: sex

>   male 17080

>   female 15981

>   Name: count, dtype: int64 --- sex

>   male 17145

>   female 15981

>   Name: count, dtype: int64

>   age_approx: age_approx

>   45.0 4466

>   50.0 4270

>   55.0 3824

>   40.0 3576

>   60.0 3240

>   35.0 2850

>   65.0 2527

>   30.0 2358

>   70.0 1968

>   25.0 1544

>   75.0 981

>   20.0 655

>   80.0 419

>   85.0 149

>   15.0 132

>   90.0 80

>   10.0 17

>   0.0 2

>   Name: count, dtype: int64 --- age_approx

>   45.000000 4466

>   50.000000 4270

>   55.000000 3824

>   40.000000 3576

>   60.000000 3240

>   35.000000 2850

>   65.000000 2527

>   30.000000 2358

>   70.000000 1968

>   25.000000 1544

>   75.000000 981

>   20.000000 655

>   80.000000 419

>   85.000000 149

>   15.000000 132

>   90.000000 80

>   48.384641 65

>   10.000000 17

>   49.747592 3

>   0.000000 2

>   Name: count, dtype: int64

>   anatom_site_general_challenge: anatom_site_general_challenge

>   torso 16845

>   lower extremity 8417

>   upper extremity 4983

>   head/neck 1855

>   palms/soles 375

>   oral/genital 124

>   Name: count, dtype: int64 --- anatom_site_general_challenge

>   torso 17372

>   lower extremity 8417

>   upper extremity 4983

>   head/neck 1855

>   palms/soles 375

>   oral/genital 124

>   Name: count, dtype: int64

>   diagnosis: diagnosis

>   unknown 27124

>   nevus 5193

>   melanoma 584

>   seborrheic keratosis 135

>   lentigo NOS 44

>   lichenoid keratosis 37

>   solar lentigo 7

>   cafe-au-lait macule 1

>   atypical melanocytic proliferation 1

>   Name: count, dtype: int64 --- diagnosis

>   unknown 27124

>   nevus 5193

>   melanoma 584

>   seborrheic keratosis 135

>   lentigo NOS 44

>   lichenoid keratosis 37

>   solar lentigo 7

>   cafe-au-lait macule 1

>   atypical melanocytic proliferation 1

>   Name: count, dtype: int64

>   benign_malignant: benign_malignant

>   benign 32542

>   malignant 584

>   Name: count, dtype: int64 --- benign_malignant

>   benign 32542

>   malignant 584

>   Name: count, dtype: int64

>   target: target

>   0 32542

>   1 584

>   Name: count, dtype: int64 --- target

>   0 32542

>   1 584

>   Name: count, dtype: int64

>   Descriptive statistics df1:

>   age_approx target

>   count 33058.000000 33126.000000

>   mean 48.870016 0.017630

>   std 14.380360 0.131603

>   min 0.000000 0.000000

>   25% 40.000000 0.000000

>   50% 50.000000 0.000000

>   75% 60.000000 0.000000

>   max 90.000000 1.000000

>   Descriptive statistics df2:

>   age_approx target

>   count 33126.000000 33126.000000

>   mean 48.869143 0.017630

>   std 14.365611 0.131603

>   min 0.000000 0.000000

>   25% 40.000000 0.000000

>   50% 50.000000 0.000000

>   75% 60.000000 0.000000

>   max 90.000000 1.000000

>   Top Five Rows df1:

>   image_name patient_id sex age_approx anatom_site_general_challenge

>   0 ISIC_2637011 IP_7279968 male 45.0 head/neck \\

>   1 ISIC_0015719 IP_3075186 female 45.0 upper extremity

>   2 ISIC_0052212 IP_2842074 female 50.0 lower extremity

>   3 ISIC_0068279 IP_6890425 female 45.0 head/neck

>   4 ISIC_0074268 IP_8723313 female 55.0 upper extremity

>   diagnosis benign_malignant target

>   0 unknown benign 0

>   1 unknown benign 0

>   2 nevus benign 0

>   3 unknown benign 0

>   4 unknown benign 0

>   Top Five Rows df2:

>   image_name patient_id sex age_approx anatom_site_general_challenge

>   0 ISIC_2637011 IP_7279968 male 45.0 head/neck \\

>   1 ISIC_0015719 IP_3075186 female 45.0 upper extremity

>   2 ISIC_0052212 IP_2842074 female 50.0 lower extremity

>   3 ISIC_0068279 IP_6890425 female 45.0 head/neck

>   4 ISIC_0074268 IP_8723313 female 55.0 upper extremity

>   diagnosis benign_malignant target

>   0 unknown benign 0

>   1 unknown benign 0

>   2 nevus benign 0

>   3 unknown benign 0

>   4 unknown benign 0

>   ![A picture containing text, screenshot, display, software Description automatically generated](media/aab62ee876e312b5facd35d41a435573.png)
