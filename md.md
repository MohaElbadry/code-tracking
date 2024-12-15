# ENSET-Tutor: Recommended Java Packages and Technologies

## 1. Frontend (JavaFX)

Recommended Packages:

- javafx.application
- javafx.scene
- javafx.fxml
- javafx.stage
- javafx.scene.control
- javafx.scene.layout
  controlsfx (Extended JavaFX Controls)

### Additional UI Libraries:

- JFoenix (Material Design for JavaFX)
  - Use CSS and frameworks like JFoenix for modern styling.
- ControlsFX
- FontAwesomeFX (Icon integration)

# 2. Backend Processing

- java.util
- java.concurrent
- java.io
- java.time

### Recommended Libraries:

- Spring Boot
- Quarkus
- Micronaut
3. **Communication**:
   - Implement HTTP clients in Java to interact with back-end APIs.

## 3. LangChain

- Langchain4j (Emerging Java port)
- Custom RAG implementation
- OpenAI Java SDK
- Hugging Face Java API

Recommended RAG Implementation Libraries:

- DJL (Deep Java Library)
- OpenNLP
- Stanford CoreNLP

## 4. Vector Database Integration

### 3.4 Retrieval Systems
#### Vector Database Options:
* Pinecone
* Weaviate
* Milvus
* Chroma
* FAISS (Facebook AI Similarity Search)
* Search Engine Options:
* Elasticsearch
* Apache Solr
* Algolia
* MongoDB Atlas Search
### Java-Friendly Vector Databases:

- Pinecone Java Client
- Milvus Java SDK
- Weaviate Java Client
- FAISS (via JNI)

### Embedding Generation:

- Hugging Face Transformers
- DJL (Deep Java Library)
- TensorFlow Java

## 5. Language Model Integration

### Recommended Java LLM Options:

- OpenAI GPT API (via REST)
- Hugging Face Transformers Java
- Local model integration (ONNX/TensorFlow)
- Llama2 Java Wrapper

## 6. Multimodal Processing
3. **LLM Integration**:
   - Use LangChain to connect to OpenAI GPT models.
   - Add multimodal capabilities using models like CLIP.
   

### Image Processing:

- OpenCV Java
- ImageJ
- Apache Commons Imaging

### Vision Models:

- DJL (Deep Java Library)
- TensorFlow Java
- ONNX Runtime

## 7. Database Connectivity

### ORM and Database Libraries:

- Hibernate
- JPA
- MyBatis
- Spring Data JPA

Recommended Databases:

- PostgreSQL
- MySQL
- H2 (In-memory testing)
- MongoDB Java Driver

## 8. Dependency Management

Build Tools:

- Maven (Recommended)
- Gradle

## 9. Additional Recommended Dependencies

Logging:

- SLF4J
- Log4j2
- Logback

Testing:

- JUnit 5
- Mockito
- TestFX (JavaFX Testing)

Utilities:

- Apache Commons
- Guava
- Lombok

---
# More Outils

## Integration and Testing

2. **Unit Testing**:
   - Write test cases for both back-end and front-end modules.


## Optional Enhancements

2. **Deployment**:
   - Deploy the back-end on AWS or Azure.
   - Package the front-end as a JavaFX executable.

### Folder Structure

```
enset-chatbot/
│
├── backend/                  # Python backend
│   ├── src/                  # Core source code
│   │   ├── api/              # API endpoint handlers
│   │   │   ├── chat_routes.py
│   │   │   └── document_routes.py
│   │   ├── database/         # Database interactions
│   │   │   ├── connection.py
│   │   │   └── queries.py
│   │   ├── models/           # AI and database models
│   │   │   ├── llm_model.py
│   │   │   ├── vector_search.py
│   │   │   └── multimodal_processor.py
│   │   └── utils/            # Utility functions
│   │       ├── embeddings.py
│   │       └── helpers.py
│   ├── tests/                # Backend tests
│   │   ├── test_api.py
│   │   ├── test_models.py
│   │   └── test_utils.py
│   ├── requirements.txt      # Python dependencies
│   └── config.py             # Configuration settings
│
├── frontend/                 # JavaFX frontend
│   ├── src/                  # Source code
│   │   ├── main/java/        # Java source files
│   │   │   ├── views/        # UI views
│   │   │   │   ├── ChatView.java
│   │   │   │   └── DocumentBrowserView.java
│   │   │   ├── controllers/  # UI logic controllers
│   │   │   │   ├── ChatController.java
│   │   │   │   └── DocumentController.java
│   │   │   └── Main.java     # JavaFX application entry point
│   │   └── resources/        # UI resources
│   │       ├── fxml/         # FXML layouts
│   │       ├── css/          # Styling
│   │       └── assets/       # Icons, images
│   └── pom.xml               # Maven configuration
│
├── database/                 # Database management
│   ├── migrations/           # Schema evolution scripts
│   │   ├── 001_initial_schema.sql
│   │   └── 002_add_indexes.sql
│   ├── seed/                 # Initial data
│   │   └── sample_data.sql
│   └── config/               # DB connection configs
│       └── connection.json
│
├── docs/                     # Project documentation
│   ├── architecture.md       # System design overview
│   ├── setup.md              # Installation guide
│   ├── development.md        # Developer guidelines
│   └── user_manual.md        # End-user documentation
│
├── tests/                    # Comprehensive testing
│   ├── backend_tests/        # Python backend tests
│   ├── frontend_tests/       # JavaFX UI tests
│   └── integration_tests/    # Full system tests
│
├── .gitignore                # Git ignore file
├── README.md                 # Project overview
└── docker-compose.yml        # Container
```

