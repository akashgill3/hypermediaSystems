# Chapter 1 - Hypermedia Reintroduction
- **Hypermedia Overview:**
  - Universal technology akin to electricity.
  - Hypermedia-based systems are prevalent, utilizing HTML over HTTP in web browsers for various activities.
  - Diverse online services are delivered via hypermedia.

- **Under-Explored Hypermedia:**
  - Despite ubiquity, hypermedia's concepts are often left to specialists.
  - HTML, the most used hypermedia, is sometimes viewed negatively due to its legacy nature in modern web applications.

- **Importance of Hypermedia:**
  - Hypermedia is innovative, flexible, and essential for robust applications.
  - Encourages considering hypermedia-driven applications in modern web architecture.

- **What is Hypermedia?**
  - Non-linear media with branching via hyperlinks, expanding beyond traditional media like magazines.
  - Hypermedia controls define interaction, distinguishing hypermedia from other media.

- **Brief History of Hypermedia:**
  - Roots in Vannevar Bush's Memex concept, Ted Nelson's coinage of "hypertext" and "hypermedia," and Douglas Engelbart's demos.
  - Tim Berners-Lee's creation of the World Wide Web and Roy Fielding's REST architecture contributions.

- **Modern Implementation and HTML's Role:**
  - HTML as the most successful hypermedia enabling document links and form controls.
  - HTML evolved from read-only to interactive, facilitating web applications' development.

- **Essence of HTML as Hypermedia:**
  - Anchor tags and form tags as essential hypermedia controls.
  - Anchor tags facilitate navigation and HTTP requests in web browsers, crucial for hypermedia interaction.

- **Hypermedia Controls in Action:**
  - Anchor tags initiate HTTP GET requests for linked content, showcasing hypermedia navigation principles.

- **Hypermedia System Architecture:**
  - Hypermedia systems encompass various technologies like network protocols (HTTP), media types, servers, clients (e.g., web browsers), etc.
  - Emphasizes the importance of understanding the broader architecture for developing hypermedia-driven applications.

- **Hypermedia Controls in HTML:**
  - Anchor tags (hyperlinks) enable navigation between documents or resources via HTTP GET requests.
  - Form tags introduce interactive elements for updating resources, transforming the web into an application architecture.

- **Evolution of Hypermedia:**
  - Started as static documents (read-only) and evolved into dynamic, interactive content with form controls.
  - HTML's widespread adoption as the most used hypermedia reflects its pivotal role in web development.

- **Hypermedia Client-Server Interaction:**
  - Hypermedia clients (browsers) send HTTP requests to servers based on user interactions with hypermedia controls.
  - Servers respond with hypermedia content (HTML) to update the client's view, demonstrating a RESTful interaction model.

- **REST and Hypermedia:**
  - Roy Fielding's REST architecture defines a stateless client-server model using hypermedia controls for application state transitions.
  - Hypermedia (like HTML) plays a central role in RESTful web architectures, enabling dynamic application behavior.

- **Importance of Understanding Hypermedia:**
  - Hypermedia's fundamental concepts, controls, and interactions are critical for designing modern web applications.
  - Encourages developers to appreciate hypermedia's role beyond legacy perceptions and embrace its potential for innovative application design.

**Hypermedia-Driven Applications (HDAs):**

- **Simplicity and Tolerance:** HDAs are praised for their simplicity and tolerance towards content and API changes. They are often favored for applications that do not require extensive user interactivity but rely more on server-side functionality.
  
- **Benefits of Large-Grain Hypermedia Data Transfers:** The ability of HDAs to exchange hypermedia with the server using basic controls like anchor tags and forms is emphasized. This approach aligns with Roy Fielding's vision of RESTful architectures and is seen as a robust, tried-and-true method.

- **Usability Improvements with htmx:** The introduction of libraries like htmx extends the capabilities of HDAs, allowing for finer-grained hypermedia transfers and enhancing the user interface without compromising the core hypermedia architecture.

- **Simplification and Coherence:** By adopting a hypermedia-first approach and leveraging hypermedia-oriented libraries, developers can simplify their web applications, make them more coherent, and reduce the complexity associated with client-side JavaScript frameworks.

**JavaScript-Driven Single Page Applications (SPAs):**

- **Interactive User Experiences:** SPAs are lauded for offering highly interactive and immersive user experiences, with the ability to update elements on a page smoothly without full document reloads, use CSS transitions for visual effects, and respond to various user events.

- **JavaScript Fatigue:** JavaScript fatigue due to the complex infrastructure required to manage them, constant changes in JSON APIs, and the overall complexity of modern web development.

- **Exponential Complexity Growth:** Complexity in software tends to grow exponentially, making it challenging to maintain and manage large-scale SPAs over time.

**Choosing Between Hypermedia and SPAs:**

- **Appropriate Use Cases:** The decision between HDAs and SPAs depends on the specific requirements of the application. HDAs are recommended for applications where extensive user interactivity is not necessary, focusing more on server-side functionality. In contrast, SPAs excel in providing dynamic and interactive user experiences but come with increased complexity and management overhead.

- **Consideration of Complexity Budget:** The concept of a "complexity budget" is introduced, highlighting the importance of managing complexity in software development and making informed decisions about when to adopt hypermedia-driven approaches or SPAs based on the application's needs.

**'<div> Soup'**

- **Issues with Generic Elements:** The text discusses the common practice of using generic `<div>` and `<span>` elements instead of more meaningful tags, which can lead to "div soup" in HTML code. It highlights the drawbacks of such practices, including reduced accessibility and readability, as well as increased complexity in editing and debugging code.

- **Example of Improper Usage:** An example is given where a `<div>` element is used as a button with an `onclick` event handler, lacking focusability and accessibility features compared to a proper `<button>` element.

- **Improving Accessibility and Readability:** The passage suggests ways to improve the accessibility and readability of code, such as adding `role="button"` and `tabindex="0"` attributes to `<div>` elements used as buttons. It encourages developers to explore the HTML specification for appropriate tags and attributes to avoid "div soup" and ensure better code quality.

- **Benefits of Using Designated Tags:** Using designated HTML elements not only improves accessibility and semantic structure but also makes the code easier to understand, edit, and maintain. It promotes using HTML elements appropriately to enhance the overall quality of web development projects.
