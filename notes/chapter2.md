# Chapter 2 - Components of a Hypermedia System
**Hypermedia System Components:**

1. **Hypermedia**: HTML is a primary example, enabling non-linear communication between clients and servers through hypermedia controls like anchors and forms.

2. **Network Protocol**: HTTP (Hypertext Transfer Protocol) facilitates communication between clients and servers, crucial for web-based hypermedia systems.

3. **Server**: Presents a hypermedia API, responding to network requests with hypermedia responses, essential for delivering content and functionality.

4. **Client**: Interprets hypermedia responses, allowing users to interact dynamically with the system beyond linear reading.

**Hypermedia System Implementation Overview:**

- **Theoretical Foundation**: Explores concepts from Roy Fielding's dissertation, including REST (REpresentational State Transfer) and HATEOAS (Hypermedia As The Engine Of Application State), providing insight into the web's architectural underpinnings.
- **Hypermedia Controls**: Enables dynamic, non-linear interactions within hypermedia, extending beyond traditional linear reading experiences.

**URL Structure and Functionality:**

- **Uniform Resource Locator (URL)**: Defines network locations and mechanisms for resource retrieval, comprising components like scheme, userinfo, host, port, path, query, and fragment.
- **URL Components**: Schematic breakdown of a URL, with various subcomponents that may be omitted based on context.
- **Hypermedia References in HTML**: Examples of anchor tags with URLs, showcasing how hypermedia references are embedded in HTML documents.

**Hypermedia Protocols and HTTP Interaction:**

- **HTTP Usage**: Facilitates transfer of hypermedia (HTML) between clients and servers, integral to web's distributed hypermedia system.
- **HTTP Methods**: GET, POST, PUT, PATCH, DELETE; each method serves distinct purposes in resource retrieval, mutation, and deletion.
- **HTTP Requests and Responses**: Detailed breakdown of HTTP requests (e.g., `GET /book/contents/ HTTP/1.1`) and responses (e.g., `HTTP/1.1 200 OK`), including headers and content.

**Hypermedia System Challenges and Workarounds:**

- **HTTP Methods and Hypermedia Controls**: Limitations of native HTML controls (anchors, forms) to issue only GET and POST requests, necessitating JavaScript for PUT, PATCH, DELETE operations.
- **HTML Limitations**: Shortcomings in HTML's hypermedia capabilities, prompting discussions on potential improvements and workarounds.

**HTTP Response Codes and Caching:**

- **HTTP Response Codes Overview**: Numeric values indicating the result of an HTTP request, categorized into informational, successful, redirection, client error, and server error responses.
- **Common Response Codes**:
  - 200 OK: Successful request.
  - 301 Moved Permanently: Resource permanently moved to a new URL.
  - 302 Found: Resource temporarily moved to a new URL.
  - 303 See Other: Resource moved, retrieve with a GET request.
  - 401 Unauthorized: Client not authenticated for the resource.
  - 403 Forbidden: Client lacks access to the resource.
  - 404 Not Found: Requested resource not found.
  - 500 Internal Server Error: Server encountered an error processing the request.
- **HTTP Methods and Response Codes**: Utilizing appropriate methods and response codes is crucial for building a coherent hypermedia API, avoiding misuse of methods like POST and generic response codes like 200 OK.
- **Caching HTTP Responses**: HTTP allows servers to indicate cacheability of responses using headers like Cache-Control, enabling clients to cache responses for specified durations.

**Hypermedia Servers and Technology Choices:**

- **Hypermedia Servers**: Any server capable of responding to HTTP requests with HTTP responses, facilitating the creation of hypermedia-driven applications.
- **Technology Flexibility**: Adoption of hypermedia reduces backend technology constraints, allowing developers to choose backend technologies based on expertise, domain suitability, or personal preference.
- **JavaScript and Backend Pressure**: Contrasts the pressure to use JavaScript on both front end and back end in JSON Data APIs and Single Page Applications, highlighting the benefits of using hypermedia architecture.

**HOWL Stack and Universal Web Language:**

- **Hypermedia On Whatever you’d Like (HOWL) Stack**: Humorous term representing the flexibility of hypermedia-driven systems across various languages and frameworks.
- **Community Diversity**: Reflects the diverse community embracing hypermedia across languages like Ruby, Python, Lisp, Haskell, etc., fostering collaboration and support within the hypermedia architecture.
- **Universal Web Language**: Hypermedia serves as a universal language for the web, enabling interoperability and shared techniques among developers using different technologies.

**Hypermedia Clients**

Hypermedia clients, such as web browsers, are crucial components of a hypermedia system as they interpret hypermedia formats like HTML to allow users to interact with resources. While browsers are the most common hypermedia clients, other specialized clients like Hyperview for mobile exist.

**The Uniform Interface**

The Uniform Interface constraint in REST defines key principles:
- **Identification of resources**: Each resource should have a unique identifier, typically represented by URLs.
- **Manipulation of resources through representations**: Resources are represented in various formats (e.g., HTML, JSON), allowing clients to interact with them.
- **Self-descriptive messages**: Messages exchanged between clients and servers should be self-descriptive, containing all necessary information within the response.
- **Hypermedia as the engine of application state (HATEOAS)**: Hypermedia controls within responses guide clients on available actions, making the system flexible and self-describing.

**The HTML vs. JSON Example**

In a comparison between HTML and JSON representations:
- HTML embeds hypermedia controls, making clients (like browsers) aware of available actions without external knowledge.
- JSON requires clients to understand the domain model and available actions separately, leading to potential versioning and compatibility issues.

**HATEOAS and API Flexibility**

HATEOAS enables API flexibility and reduces versioning complexities:
- Hypermedia-driven APIs dynamically inform clients of available actions, eliminating the need for versioned APIs.
- Changes to APIs reflect immediately in hypermedia responses, ensuring clients stay updated without manual intervention.

**Layered System and Code-On-Demand**

REST's layered system allows intermediaries like CDNs to improve performance, while Code-On-Demand is an optional constraint allowing client functionality extension through scripts or applets.

**Conclusion**
Understanding REST's principles like the Uniform Interface and HATEOAS is essential for designing flexible and scalable hypermedia systems. Despite challenges like session management and JSON APIs' limitations, embracing hypermedia's self-descriptive nature can lead to more robust and adaptable applications.
