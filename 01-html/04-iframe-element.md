<!--Replaced Element-->

A replaced element is an element whose content is determined by an external resource rather than by CSS itself.

Common examples of replaced elements include the image, iframe, and video elements.
With replaced elements, you can control the position, or layout of an element. But your CSS cannot directly modify the content of that element.

image element, which embeds an image on your web page:
<img src="example-img-url" alt="Descriptive text goes here">

A more robust example might be the iframe element, which embeds an external site on your web page.

  <!--iframe-->

What does iframe mean?
Inline frame

<iframe width="400" height="200" 
src="https://www.youtube.com/embed/u43gJJrVa1I?si=BoDW_puFsy8OEr_Z" 
title="Professional Cloud Architect Certification Course – Pass the Exam! (YouTube video)" 
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
</iframe>

iframe element would be to embed maps onto the page.

<iframe
  title="Map of the Royal Observatory, Greenwich, London"
  width="300"
  height="200"
  src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&amp;layer=mapnik">
</iframe>

There are some other replaced elements, such as video, and embed. And some elements behave as replaced elements under specific circumstances.

The src attribute specifies the URL of the page you want to embed.
The width attribute specifies the width of the iframe.
The height attribute specifies the height of the iframe.
The allowfullscreen attribute allows the user to display the iframe in full screen mode.

The allow attribute, on the other hand, lets you define what an iframe can or can't do. This is called an allowlist. In the above example, adding clipboard-write to it allows the embedded page to write items to your clipboard.

If you want to embed direct HTML within the iframe element you have to use the srcdoc attribute instead of src.
