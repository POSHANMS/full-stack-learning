<!--Div elements-->
<p>The div element has no semantic meaning.</p>
  <p>Example paragraph element.</p>
  <p>Example paragraph element.</p>
  <p>Example paragraph element.</p>
</div>
<hr>

<!--Section elements over Div-->
<section>
  <h2>Mammals</h2>
  <p>
    Mammals are warm-blooded animals with fur or hair. Most give birth to live
    young.
  </p>
  <ul>
    <li>Lion</li>
    <li>Elephant</li>
    <li>Dolphin</li>
  </ul>
</section>
<p>The section element has semantic meaning over the div element which is not semantic. Semantics are the meaning of words or phrases in a language. In HTML, which is a language, elements have their own semantic meaning too. So, this means if you use a section element, the browser will pick up its semantic meaning and understand to treat this as a section - on desktops, mobiles</p>
<hr>

<!--Id attribute-->
<p>The id attribute adds a unique identifier to an HTML element.</p>
<h1 id="title">Movie Review Page</h1>
<h2 id="subtitle">Movies</h2>
<p>Browsers will see this space as part of the id which will lead to unwanted issues when it comes to styling and scripting. id attribute values should only contain letters, digits, underscores, and dashes.</p>
<hr>

<!--Class attribute-->
<p>In contrast to the id attribute, the class attribute value does not need to be unique and can contain spaces.</p>
<div class="box"></div> <!--.box { width: 100px; height: 100px; }-->
<div class="box red-box"></div><!--.red-box { background-color: red; }-->
<div class="box blue-box"></div><!--.blue-box { background-color: blue; }-->
<p>when should you use an id versus a class? Classes are best used when you want to apply a set of styles to many elements. If you want to target a specific element, it is best to use id because those values need to be unique.</p>
<hr>

<!--HTML Entites-->
<p>An HTML entity, or character reference, is a set of characters used to represent a reserved character in HTML.</p>
&lt;p&gt;learning is fun&lt;/p&gt;
<p>These types of character references are known as named character references.</p>
<p>Named references start with an ampersand sign (&) and end with a semicolon (;). By using a named character reference, the HTML parser will not confuse this with an actual HTML element.</p>
<p>Another type of character reference would be the decimal numeric reference. This character reference starts with an ampersand sign and hash symbol (#), followed by one or more decimal digits, followed by a semicolon.</p>
&#60; <!--For < -->
&#169;
&#174;
<p>hexadecimal numeric reference character reference starts with an ampersand sign, hash symbol, and the letter x. Then it is followed by one or more ASCII hex digits and ends with a semicolon. </p>
&#x3C;
<hr>

<!--Role of Script Element-->
<p>The script element is used to embed executable code. Most developers will use this to execute JavaScript code. JavaScript is used to add interactivity to your web pages. Common examples of using JavaScript include interactive games, image sliders, and dynamic forms that validate user input in real-time.</p>
<body>
  <script>
    //alert("Welcome to freeCodeCamp");
  </script>
</body>
&lt;script src="path-to-javascript-file.js"></script&gt;>
<br>
<p>The src attribute is used here to specify the location for that external JavaScript file. src stands for "source". The reason why it is not encouraged to place all of your JavaScript inside the HTML document is because of separation of concerns. </p>

<!--Ordered lists-->

Ordered lists in HTML are used to display a series of items in a specific order. Each item in the list is typically numbered, allowing readers to easily follow a sequence or ranking. The <ol> tag is used to create an ordered list, and each list item is defined using the <li> tag.

<!--Unordered Lists-->

Unordered lists present items in a bulleted format, where the order of the items is not significant. They are used to group related content together without implying any specific sequence or priority. Each item in the list is typically marked with a bullet point, making it easy to visually distinguish and scan the list's contents.

<!--Definition Lists-->

Definition lists in HTML are used to present terms and their corresponding definitions. They are structured using three main elements: <dl> (definition list), <dt> (definition term), and <dd> (definition description). The <dl> element acts as the container for the entire list, while each term is marked with <dt> and its associated description is enclosed within <dd>. This structure allows for a clear and organized presentation of terms and their meanings.

<!--Nested Lists in HTML-->

Nested lists in HTML allow you to create lists within lists, forming a hierarchical structure. This is achieved by placing one list (either ordered <ol> or unordered <ul>) inside a list item <li> of another list. This creates a sub-list that is visually indented, helping to organize information into related categories and subcategories.

<!--Priority Hints-->

Priority Hints in HTML allow developers to indicate the relative priority of fetching resources like images. This helps the browser decide which images to load first, potentially improving page load times and user experience by prioritizing content that is immediately visible or more important to the user. This is achieved using the fetchpriority attribute.
