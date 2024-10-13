## Introduction

Historically, **artificial intelligence (AI)** and **machine learning (ML)** were not accessible to most people. Only specialized engineers, who were few and expensive to hire, could develop these solutions. However, ML is now **more accessible** than ever, enabling a wider range of people to build models, even without technical expertise.

**Google Cloud offers four options** for building machine learning models:

1. **BigQuery ML**: 
   - Use **SQL queries** to create and execute ML models directly in BigQuery.
   - Ideal if your data is already in BigQuery and your problems fit predefined ML models.

2. **Pre-trained APIs**: 
   - Utilize ML models developed and trained by Google.
   - A good option if you lack training data or sufficient ML expertise.

3. **AutoML**: 
   - A **no-code solution** that allows you to build ML models on Vertex AI using a point-and-click interface.

4. **Custom Training**: 
   - Provides the ability to code your own ML environment, including training and deployment.
   - Offers **flexibility** and **control** over the ML pipeline.

In the next section of the course, you will explore these four options in more detail and learn about additional AI solutions from Google.

## BigQuery ML

**Machine learning** on large data sets typically requires **extensive programming** skills and knowledge of ML frameworks, limiting development to a small group within companies. This often excludes **data analysts** who understand the data but lack programming expertise.

**BigQuery** has evolved from being just a data warehouse to supporting the entire data-to-AI lifecycle. **BigQuery ML** democratizes machine learning by allowing data analysts to build and run models using existing **business intelligence tools** and spreadsheets.

Key benefits of BigQuery ML include:

- **No need for programming**: Models are trained using SQL, a familiar language for data analysts, eliminating the need for Python or Java.
- **Predictive analytics**: This can guide business decision-making across the organization.
- **Reduced complexity**: Fewer tools are required for model development.
- **Increased speed**: There's no need to move or format large data sets for traditional Python-based ML frameworks.

Additionally, BigQuery ML integrates with **Vertex AI**, Google Cloud's end-to-end AI platform. Models created in BigQuery ML can be registered in the **Vertex AI model registry** and deployed for **online predictions**.

## Pre-trained APIs

**Google Cloud's pre-trained APIs** are ideal for organizations that lack their own training data and specialized data scientists but have business analysts and developers. 

Key features include:

- **Fastest and lowest effort** approach to machine learning, although less customizable than other options.
- Helps developers quickly build smart applications by providing access to ML models for common tasks, such as **image, video, and text analysis**.
- APIs can be deployed in various environments: **virtual private cloud, on-premises, or Google’s public cloud**.

### Examples of Pre-trained APIs:

1. **Vision API**: 
   - Used for image recognition and filtering (e.g., detecting faces, objects, and sentiment).
   - Can automatically classify images into millions of predefined categories.

2. **Natural Language API**: 
   - Analyzes text from contact forms, discovering syntax, entities, and sentiment.
   - Classifies text into categories like complaints or praise.

3. **Other APIs**:
   - **Cloud Translation API**: Converts text between languages.
   - **Speech-to-Text API**: Converts audio into text for data processing.
   - **Text-to-Speech API**: Converts text into high-quality voice audio.
   - **Video Intelligence API**: Recognizes motion and action in videos.

The effectiveness of these models is supported by Google's extensive data and research, providing **faster returns on investment** with less effort required from users.

## Auto ML

Another custom way to use machine learning is by training models with your own data through **Vertex AI**. This platform unifies Google Cloud services for building ML projects under a single user interface. 

Key features include:

- **AutoML**: Allows users to build and train machine learning models using graphical user interfaces (GUIs) without coding. After data ingestion, AutoML selects the best model and tunes parameters automatically, resulting in accurate, customized models.
- This approach enables practitioners to focus on problem-solving rather than the technical details of ML.

For instance, a car manufacturer could use **AutoML Vision** to train a model to distinguish between good and defective parts using their specialized image data, rather than relying on generic models like Vision API.

Similarly, **AutoML Natural Language** allows users to build custom models for document analysis, categorization, entity recognition, and sentiment assessment, all through an easy-to-use interface without coding.

Vertex AI supports a variety of ML applications, including video categorization, audio-to-text conversion, natural language understanding, and translation, often combining multiple applications for innovative solutions.

## Custom models

Vertex AI is the key platform for creating custom end-to-end machine learning models, allowing models to be trained and tailored with your own data. It offers a comprehensive suite of products that support each stage of the ML workflow, including data gathering, feature engineering, model building, deployment, and monitoring.

While this fully custom approach requires a specialized team of data scientists and engineers and takes longer to implement, it results in highly specialized models that provide significant differentiation and innovative outcomes for businesses. Vertex AI includes tools for virtual machine imaging, data labeling, training, and predictions, along with pre-built algorithms. However, it's crucial to note that there is no one-size-fits-all solution; each use case demands a unique combination of tools and products.

## TensorFlow

All machine learning models on Google Cloud are built on its foundational AI infrastructure, which includes TensorFlow. Key points include:

- **TensorFlow Overview**: An end-to-end open-source platform for machine learning that provides a flexible ecosystem of tools, libraries, and community resources for researchers and developers.
- **Development History**: Originally developed for internal use at Google, TensorFlow is now available to the public to facilitate broader innovation.
- **TPUs (Tensor Processing Units)**: Custom-developed application-specific integrated circuits designed to accelerate ML workloads. TPUs are more efficient than general-purpose CPUs and GPUs.
- **Performance Advantage**: TPUs significantly increase computing speed—over 200 times faster than traditional GPUs, reducing processing time from 26 hours to approximately 7.9 minutes for complex tasks.
- **Integration**: Cloud TPUs are integrated across various Google products, providing state-of-the-art hardware and supercomputing capabilities within Google Cloud services.

## AI solutions

Google Cloud offers a range of full AI solutions tailored to specific business needs:

- **Contact Center AI**: Enhances customer interactions by providing models that assist human agents and improve operational efficiency, personalizing customer care.
- **Document AI**: Extracts and classifies information from unstructured documents (e.g., invoices, receipts) for storage in databases or further analysis.
- **Discovery AI for Retail**: Optimizes product ordering on e-commerce sites based on historical data, improving the visibility and sales likelihood of products in specific categories.
- **Cloud Talent Solution**: Utilizes AI to streamline job search and talent acquisition, matching candidates with suitable jobs and helping employers attract quality talent.

These solutions are designed to meet various operational challenges across industries.

## Considerations when selecting Google Cloud AI/ML solutions

When selecting AI and ML solutions from Google Cloud, several key considerations and trade-offs arise:

1. **Speed**: The time to get a model into production can range from 3 to 36 months, depending on the project's complexity. Pre-trained APIs require no model training, making them the fastest option, while custom training takes the longest due to the need to build models from scratch.

2. **Differentiation**: Organizations must consider how unique their models need to be. Google Cloud offers ready-to-use solutions for quick deployment, such as image recognition and chatbots. For more tailored solutions, Vertex AI provides a platform for custom model training, giving engineers full control over the workflow.

3. **Expertise Required**: Successful AI integration necessitates roles such as data engineers, data scientists, and ML engineers. Organizations should evaluate their current team and strategize accordingly, whether through upskilling, repurposing resources, or hiring external consultants.

4. **Effort to Build**: The effort needed depends on problem complexity, data availability, and team experience. Google Cloud supports projects of varying scales, but significant time, effort, and expertise are essential for impactful AI implementations.