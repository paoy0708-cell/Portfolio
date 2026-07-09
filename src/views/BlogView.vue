<template>
  <div class="container mx-auto p-3 md:p-8">
    <div class="flex flex-col-reverse md:flex-row relative">
      <div class="w-full">
        <div class="flex flex-col gap-4 md:px-20 fade-zoom-up">
          <article v-for="article in articles" :key="article.id">
            <router-link
              :to="`/read/${article.slug}/${article.id}`"
              class="flex w-full bg-[#1e1e1f] border-[#383838] rounded-xl text-left text-white p-5 md:py-7 md:px-8 cursor-pointer hover:bg-[#282828] items-center"
            >
              <div class="w-full pr-4 bg-[#1e1e1f] border-[#383838]">
                <div
                  class="text-xs mb-1 text-slate-400 flex items-center italic"
                >
                  <div
                    class="h-[1px] w-20 bg-amber-200 md:w-5 aos-init aos-animate mr-2"
                  ></div>
                  {{ article.date }}
                </div>
                <h1
                  class="text-sm md:text-md text-amber-200 font-bold mb-2 paraf"
                >
                  {{ article.title }}
                </h1>
                <div class="text-sm text-amber-200 md:block paraf">
                  {{ article.desc }}
                </div>
                <div class="text-sm hidden md:block paraf">
                  {{ article.skills }}
                </div>
              </div>
            </router-link>
          </article>
        </div>
      </div>
    </div>
  </div>
  <ArticleList />
</template>

<script>
import ArticleList from "@/components/ArticleList.vue";
export default {
  data() {
    return {
      articles: [
        {
          title: "AI Engineer",
          desc: "Listen Labs (Startup),San Francisco, California",
          slug: "aspernatur-eos-perspiciatis",
          date: " Aug 2023 - June 2025",
          skills:
            "Hugging Face, Transformers, PU learning, Natural language processing, NLTK, spacy, topic modelling, Sentiment analysis, Word Embedding, scikit-learn, Spring Boot, Django, React, Next.js, PostgreSQL, RPC, gRPC, AWS, GCP, SageMaker, Glue, ETL, PU learning",
          content:
            "•Redesigned and optimized data pipelines to unify subscription KPIs across multiple streaming platforms, collaborating with domain experts to refine data models and analytics frameworks.<br/>•Developed Python-based ETL APIs, reducing overall processing time by 30% on AWS-based infrastructure.<br/>•Led a team of 5 software engineers to build and deploy an end-to-end heart condition detection system that achieves 94.27% accuracy; it records heart sounds with a simple stethoscope and analyzes the clips in Keras and TensorFlow.<br/>•Designed a scalable architecture with a real-time NLP engine, content management system, analytics dashboard, and one-click deployment module.<br/>•Trained deep neural nets on the cleaned clips, which raised accuracy and cut false positives by 20%.<br/>•Drove another 15% lift by pairing those networks with SVM, KNN, and trees, then tuning them on over sampled data through grid search.<br/>•Leveraged Databricks for distributed data processing and collaborative development, reducing data pipeline latency, and accelerating iteration speed by approximately 40% in the ML lifecycle.<br/>•Developed a machine learning model to identify high-propensity prescribers (HCPs) for a newly launched oncology drug, leveraging Positive-Unlabeled (PU) learning techniques to handle data imbalance.<br/>•Designed and trained a GENPU GAN-based model, improving precision and recall for more effective targeting. Automated model retraining using AWS SageMaker, Glue, and Redshift, integrating real-time insights into an nteractive dashboard for sales teams.<br/>•Integrated machine learning inference services into a Python, Java backend, enabling real-time predictions delivered to a Javascript frontend.<br/>•Optimized API design and data serialization to minimize latency and support scalable user interactions.",
          id: "1",
        },
        {
          title: "AI Engineer",
          desc: "Google, San Jose, CA",
          slug: "neque-dicta-eaque",
          date: "Jan 2021 - July 2023",
          skills:
            "AWS, Kinesis, Glue, DynamoDB, and QuickSight, Hugging Face, Transformers, OpenAI,  Natural language processing, NLTK, RAG, Pytorch, Tensorflow, CNN, spacy, scikit-learn, Nvidia NeMo,ANs, PU learning, LLMs, ETL, Spring   Boot, Django, GoLang, React, Vue, PostgreSQL, RPC, gRPC,  CI/CD, GCP, Azure, Redshift",
          content:
            "•Developed and deployed a Conversational AI chatbot using Nvidia NeMo and AWS, integrating speech-to-text models to enhance natural language understanding.<br/>•Leveraging LangChain,I effectively manage interactions with language models, orchestrate omponents across the workflow, and integrate external resources and databases with ease and efficiency.<br/>•Optimized the pipeline to reduce latency by 35% and improve response accuracy.<br/>•Architected and productionized an end-to-end Conversational AI system leveraging AWS, Kinesis, Glue, DynamoDB, and QuickSight,  enabling real-time customer interactions and analytics.<br/>•Developed an automated age-based diagnostic system for lung inflammation detection using real X-ray images, leveraging advanced image processing techniques, segmentation methods, and deep learning models. ine-tuned d trained a custom CNN model, optimizing feature extraction and classification accuracy for improved medical diagnosis.<br/>•Steered product management for 'Compliance AI CoPilot' in developing harmonious design, resolution of issues, and feature prioritization for enterprise applications of generative AI.<br/>•Refined and modernized the extraction of meta-data entities by applying few-shot learning, in-context learning, and recursive reasoning techniques.<br/>•Engineered AI frameworks using cutting-edge LLMs, and retrieval-augmented generation for enterprise applications.<br/>• Acquired experience in Azure, OpenAI, and advanced AI concepts, including vector indexing, data ingestion, and entity categorization.<br>•Designed a scalable architecture with a real-time NLP engine, Hugging ce, content management system, analytics dashboard, and one-click deployment module.<br/>•Integrated machine learning and NLP models into a Go, Python backend, exposing scalable inference APIs consumed by Javascript frontends; streamlined data flow and optimized API design to reduce latency and enhance user experience.<br/>•Designed and deployed end-to-end model serving pipelines, connecting real-time ML predictions with web applications; leveraged cloud services and CI/CD practices to enable seamless updates and ensure high availability in production environments.",
          id: "2",
        },
        {
          title: "Machine Learning Research Intern",
          desc: "Google, San Jose, CA",
          date: " Jan 2020 - Dec 2020",
          skills:
            "Hugging Face, Transformers, OpenAI,  RAG, Pytorch, Tensorflow, CNN, Natural language processing, NLTK,scikit-learn, LLMs, ETL, AWS",
          slug: "cumque-error-sapiente",
          content:
            "•Conducted in-depth study and research on Deep Learning and Neural Networks, focusing on state-of-the-art methodologies and techniques in the field.<br/>•Executed hands-on experimentation with various Deep Learning frameworks and libraries, including TensorFlow, PyTorch and Keras, to gain practical insights into model development and optimization.<br/>•Applied theoretical knowledge to design and implement a basic Convolutional Neural etwork (CNN) architecture tailored for recognizing handwritten digits.<br/>•Utilized Python programming language along with relevant libraries such as NumPy and Matplotlib to preprocess datasets and visualize model performance metrics.<br/>•Implemented data augmentation techniques to enhance the robustness of the CNN model and improve its generalization ability across diverse handwriting styles.<br/>•Fine-tuned hyperparameters and conducted systematic model validation to optimize the performance of the CNN, achieving notable accuracy in digit recognition tasks.<br/>•Collaborated with senior researchers and engineers to discuss findings, troubleshoot challenges, and refine the architecture of the CNN model for improved accuracy and efficiency.<br/>•Documented the entire development process, including model architecture, training procedures, and experimental results, in a comprehensive report for knowledge sharing and future reference.<br/>•Presented research findings and project outcomes to internal stakeholders, showcasing the effectiveness and potential applications of the developed CNN model in real-world scenarios.",
          id: "3",
        },
        {
          title: "Full-Stack & AI Engineer",
          desc: "OpenSpace (Startup), San Francisco, CA",
          date: "Jul 2017 - Dec 2019",
          skills:
            "React, Angular, Nest.js, Next.js, .NET, AWS, Ruby on Rails, Python ,Hugging Face, Transformers, OpenAI,  Natural language processing, NLTK, RAG, Pytorch, Tensorflow, CNN, spacy, scikit-learn, Nvidia NeMo,ANs, PU learning, LLMs, ETL, Spring   Boot, Django, GoLang,",
          slug: "ut-ad-consequuntur",
          content:
            "•Built ML infrastructure with Golang, Docker, Databricks, Kubernetes.<br/>•Developed backend logic for LLM pipelines with PyTorch, Spark, Pandas.<br/>•Added LLM safety features using Hugging Face.<br/>•Deployed using blue-green deployments and rolling updates in EKS.<br/>•Built monitoring dashboards with Grafana and Prometheus.<br/>•Managed secrets with AWS Secrets Manager.<br/>•Tuned auto-scaling, cutting infra costs by ~20%.<br/>•Automated testing with NUnit, Selenium.<br/>•Monitored systems with AWS CloudWatch, Prometheus alerts.<br/>•Automated backup & recovery with AWS Backup, RDS snapshots.<br/>•Stored documents securely on AWS S3 (HIPAA compliance).<br/>•Developed scalable backend services in Node.js, PHP, Django, FastAPI, Flask; managed 1M+ monthly API requests.<br/>•Built dashboards with React and Next.js, improving client decision-making speed by 25%.<br/>•Automated CI/CD using GitLab and Jenkins, improving code coverage and cutting deployment errors by 35%.<br/>•Enhanced Kubernetes logging and alert systems, improving stability by 40%.<br/>•Developed and maintained enterprise healthcare web applications for lab workflow automation, digital client portals, and online reporting - using Django, Flask, and SQL Server for backend systems.<br/>•Designed and optimized SQL Server stored procedures, indexing strategies, and data models to support high-volume transactional processing of lab orders, test results, and reporting pipelines.<br/>•Delivered Single Page Applications (SPA) with AngularJS and jQuery, enhancing internal lab staff productivity and improving test result turnaround times.<br/>•Maintained and extended legacy WCF services and SOAP APIs for integration with EMR systems and external lab partners, applying WS-Security and HIPAA-compliant encryption and data handling.<br/>•Integrated RabbitMQ with Node.js services to support real-time processing of lab order events,result notifications, and system alerts across multiple applications.<br/>•Developed reusable front-end components and shared UI libraries to standardize presentation across client and internal lab applications.<br/>•Wrote automated unit tests and integration tests using NUnit, contributing to regression prevention and improving release quality.<br/>•Participated in Agile delivery cycles, working closely with business stakeholders and QA to deliver iterative enhancements to critical lab applications.<br/>•Supported CI/CD pipelines using Team Foundation Server (TFS) and MSBuild, improving deployment consistency and reducing cycle times for production releases.<br/>•Built application monitoring and centralized logging with ELK Stack (Elasticsearch, Logstash,Kibana), enhancing production support and troubleshooting capabilities.",
          id: "4",
        },
      ],
    };
  },
  components: {
    ArticleList,
  },
};
</script>

<style scoped>
.paraf {
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  text-overflow: ellipsis;
  overflow: hidden;
}
@media (min-width: 768px) {
  .paraf {
    display: -webkit-box;
  }
}
@keyframes fadeZoomUp {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}
.fade-zoom-up {
  animation: fadeZoomUp 1s ease-in-out;
  /* animation-delay: 1000ms; */
}
</style>
