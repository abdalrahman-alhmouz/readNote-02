## what ilearnd today ? 
# How to change image size in CSS?

> *Sometimes, it is required to fit an image into a certain given dimension. We can resize the image by specifying the width and height of an image. A common solution is to use the max-width: 100%; and height: auto; so that large images do not exceed the width of their container. The max-width and max-height properties of CSS works better, but they are not supported in many browsers.And You can control the size of an image using the width and height properties in CSS,Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.*

![](https://www.miltonmarketing.com/wp-content/uploads/2018/03/mmhtmlimgtag424243image-tag-example.jpg)

> The object-fit property is generally applied to image or video. This property defines how an element responds to the width and height of its container. Mainly there are five values of object-fit property such as fill, contain, cover, none, scale-down, initial, and inherit. The default value of this property is “fill”.


# How You Can Control of Width and Height Of An Image In Css?

- The width property specifies the width of an element, and the height property specifies the height of an element.
- The width and height of the image can be specified by applying these properties to the IMG element.

*Examples:*

``` ruby
div { width: auto;
text-align: center;
padding: 15px; border: 3px solid red;
} img {
max-width: 100%;
height: auto; }
```
# Aligning images in CSS
> Rather than using the < img > element’s align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:

- The float property is added to the class that was created to represent the size of the image.

- New classes are created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.


# Repeating Images (background-repeat, background-attachment)
> ***The background-repeat property can have four values:***

- repeat: The background image is repeated both horizontally and vertically (the default way itis shown if the backgroundrepeat property isn't used).
- repeat-x: The image is repeated horizontally only (as shown in the first example on the left).
- repeat-y: The image is repeated vertically only.
- no-repeat: The image is only shown once.


> *The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:*
- fixed The background image stays in the same position on the page.

- scroll The background image moves up and down as the user scrolls up and down the page.

<hr>
# Video and Audio

~[](https://cdn-media-1.freecodecamp.org/images/1*jB3XGWVtrr8qOl21gCOAmQ.gif)

*You can review what all the HTML features do in the article linked above; for our purposes here, the most interesting attribute is controls, which enables the default set of playback controls. If you don't specify this, you get no playback controls.*

> It is a good idea to always include `width` and `height` attributes. If height and width are not set, the page might flicker while the video loads.
> The `<source>` element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.
> The text between the `<video>` and `</video>` tags will only be displayed in browsers that do not support the `<video>` element.






<hr>

# What Is SEO / Search Engine Optimization?

![](https://lh3.googleusercontent.com/proxy/gHWRTKxYiG1rXGxhBQrNntpYSrMRIQkqSQzheBa8bEGGHDi6nixnt21uVN5nv0x2txchMM5wdRa8lv5JpYi-1wa4me_S7-I1Pz4ozK7DT7NZSUwHrl5aKkJ_smFY4aNYgMHepg0-)

> SEO stands for “search engine optimization.” In simple terms, it means the process of improving your site to increase its visibility for relevant searches.
> The better visibility your pages have in search results, the more likely you are to garner attention and attract prospective and existing customers to your business.

# How does SEO work?

> You might think of a search engine as a website you visit to type (or speak) a question into a box
> and Google, Yahoo!, Bing, or whatever search engine you’re using magically replies with a long list of links to webpages that could potentially answer your question.
> ***That’s true. But have you ever stopped to consider what’s behind those magical lists of links?***

> *Here’s how it works: Google (or any search engine you’re using) has a crawler that goes out and gathers information about all the content they can find on the Internet. The crawlers bring all those 1s and 0s back to the search engine to build an index. That index is then fed through an algorithm that tries to match all that data with your query.*

![](https://www.lyfemarketing.com/blog/wp-content/uploads/2018/09/2-1.png)
