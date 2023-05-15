>   As we approach the submission of the capstone project, which reflects my culmination of learning and understanding in ML, I have realized that there is still much more to learn to effectively apply it in a real-world context.

>   For instance, I am developing the initial Pay-Per-Use dermatology Electronic Medical Record (EMR) solution specifically tailored to the Indian market. A valuable feature that would greatly benefit doctors is a patient complaint triage system. However, our platform, symabMED.in, is not yet prepared for implementation. Our system must run continuously for 12 to 18 months to gather relevant metadata and high-resolution images with accurate categorization for a real-world scenario in India. This data collection phase is crucial to ensure the effectiveness and reliability of our solution.

![A screenshot of a computer Description automatically generated with medium confidence](media/08a7bc76cabdf26c35148bb6281cfc58.png)

>   Indeed, developing a generic framework using the HAM10000 dataset in the interim would be beneficial. This dataset can be a valuable resource for training and initial system testing. Furthermore, by building and fine-tuning the framework with this dataset, you can assess its performance, make necessary improvements, and gain valuable insights before incorporating the actual data from the Indian market.

>   Once the system is ready to incorporate real-world data, you can seamlessly transition by providing the relevant and authentic data to run the first pass. This approach allows you to validate the system's performance in a more realistic context and observe how it handles the specific challenges and characteristics of the Indian market.

>   By leveraging the HAM10000 dataset initially and later integrating the actual data, you can maximize the effectiveness and accuracy of the dermatology EMR solution, ensuring it meets the specific requirements and nuances of a working system.

>   Skin cancers encompass a range of diseases marked by the presence of abnormal growths or persistent sores that do not heal, as well as alterations in the size, shape, or colour of moles. There are two primary types: melanoma (less prevalent but more hazardous) and non-melanoma skin cancers (more common but less severe).

>   Notably, India experiences a relatively lower incidence of skin cancer than Western countries. This can be attributed, in part, to individuals with darker skin being less susceptible to this condition. The higher levels of melanin in darker skin provide a certain degree of protection against damage caused by UV radiation, thereby reducing the risk of developing skin cancer

>   However, regional variations can play a role in the prevalence of skin cancer in India: our system, in addition to other standard data like age, gender and what is included in the HAM dataset, a new training data may include the following features.

>   Latitude: Regions closer to the equator receive more intense sunlight, increasing the risk of skin cancer. Hence, regions in the southern part of India may see a slightly higher incidence rate.

>   Altitude: Higher altitudes receive more UV radiation. Therefore, areas at higher elevations could potentially have a higher incidence of skin cancer.

>   Outdoor occupations: In regions where more people work outdoors (like farming communities), there are increased sun exposure and a potentially higher risk of skin cancer.

>   Urban vs rural: Urban areas might see different rates due to lifestyle differences, including more indoor work and potentially more access to healthcare for early detection.

>   Cultural and social practices: Clothing, sunscreens, and shade can vary by region and influence skin cancer rates. Some traditional attire covers much of the body, providing natural sun protection

>   I plan to develop a generic framework for my capstone project focused on feature cleaning and normalization. This framework will consist of a routine that will take inputs like DataFrame, Columns property type, and specific methods to identify and perform operations such as one-hot encoding and replacing null values. I intend to test this routine using the HAM10000 dataset from the year 2020.

>   Additionally, I will create a separate routine specifically designed to standardize the image files within the dataset. This routine will remove any records of corrupt image files, including their associated metadata. Finally, I aim to validate the effectiveness of this routine by testing it on the HAM datasets.

>   By developing and implementing these routines, I aim to enhance the quality and consistency of the metadata within the dataset, ensuring that it is well-organized and suitable for further analysis. In addition, the image standardization routine will enable the removal of corrupt image files, ensuring that the dataset remains reliable and accurate for subsequent image-based analysis and processing.

>   As part of your capstone project, you have outlined a comprehensive plan. The generic framework you intend to build will generate pre and post-reports, allowing for an assessment of the data before and after the cleaning and normalization processes. Additionally, you aim to include a validation of the row data, providing an opportunity to examine individual records in the dataset. This framework will ultimately result in a finalized dataset that can be used to identify a suitable machine-learning model. Finally, I plan to evaluate the performance of the selected model against a separate test dataset, specifically the HAM10000 2020 test dataset.

>   Furthermore, I will write pre and post-reports, documenting the steps taken and the outcomes of the data preparation and cleaning processes. The inclusion of visitation allows for a more thorough understanding of the dataset and potential insights derived from individual records.

>   If all components of the project work as intended, you will have a comprehensive codebase capable of handling any DataFrame for image classification. Furthermore, the framework will facilitate data visualization and preparation for ML modelling, including selecting appropriate models. Additionally, you aim to provide an API that can be utilized as a real-world service.

>   By following this plan, I will have a robust solution that streamlines the entire process, from data preprocessing to model selection, enabling an image classification service deployment through the API.
