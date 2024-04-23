# QuizApp
The Quiz-App is a microservice-based architecture that consists of multiple services designed to handle different aspects of the quiz application. It is built using Spring Boot and incorporates Eureka Server for service discovery, OpenFeign for communication between services, and an API Gateway for centralized routing.<br/>
Architecture Overview The Quiz-App architecture is based on microservices, where each service is responsible for a specific domain or functionality. <br/>The key components of the architecture include:<br/>
Eureka Server: The service registry that allows microservices to discover and communicate with each other.<br/>
Quiz Service: A microservice that handles quiz-related operations, such as creating quizzes, managing questions, and evaluating quiz results.<br/>
Question Service: A microservice responsible for managing question-related operations, including adding new questions, retrieving question details, and maintaining question categories.<br/>
API Gateway: The centralized entry point for all client requests. It acts as a reverse proxy, routing requests to the appropriate microservices.<br/><br/>
Services Description<br/>
1.	Eureka Server Endpoint: http://eureka-server:8761/ Description: The Eureka Server provides a registry of all microservices in the system, allowing each service to discover and communicate with others.<br/>
2.	Quiz Service Endpoint: http://quiz-service:8081/ Description: The Quiz Service manages quiz-related functionalities. It exposes REST APIs for creating quizzes, managing questions, and evaluating quiz results.<br/>
3.	Question Service Endpoint: http://question-service:8082/ Description: The Question Service handles question-related operations. It provides APIs for adding new questions, retrieving question details, and managing question categories.<br/>
4.	API Gateway Endpoint: http://api-gateway:8765/ Description: The API Gateway serves as a single entry point for all client requests. It routes incoming requests to the appropriate microservices and handles cross-cutting concerns like authentication, logging, and monitoring. <br/>
