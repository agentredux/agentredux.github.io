<!--- This is a YAML Front Matter --->

---
title: "Gallery : Template"
categories:
  - Template
tags:
  - gallery
  - Post Formats
  - tiled
  
<!--- When you have the images in the '/images' folder --->
gallery:
  - url: unsplash-gallery-image-1.jpg
    image_path: unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: unsplash-gallery-image-2.jpg
    image_path: unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: unsplash-gallery-image-3.jpg
    image_path: unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
    title: "Image 3 title caption"
  - url: unsplash-gallery-image-1.jpg
    image_path: unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 4"
    title: "Image 4 title caption"
  - url: unsplash-gallery-image-2.jpg
    image_path: unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 5"
    title: "Image 5 title caption"
  - url: unsplash-gallery-image-3.jpg
    image_path: unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 6"
    title: "Image 6 title caption"
	
<!--- When you have the link to the image, and the Source URL --->
gallery2:
  - url: https://flic.kr/p/8a6Ven
    image_path: https://farm2.staticflickr.com/1272/4697500467_8294dac099_q.jpg
    alt: "Black and grays with a hint of green"
  - url: https://flic.kr/p/8a738X
    image_path: https://farm5.staticflickr.com/4029/4697523701_249e93ba23_q.jpg
    alt: "Made for open text placement"
  - url: https://flic.kr/p/8a6VXP
    image_path: https://farm5.staticflickr.com/4046/4697502929_72c612c636_q.jpg
    alt: "Fog in the trees"
	
	
<!--- Similar to the first Gallery --->
gallery3:
  - image_path: unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
  - image_path: unsplash-gallery-image-4-th.jpg
    alt: "placeholder image 4"
---

<!--- The three dashes above indicate start/end of YAML front matter, and is necessary for every file we make --->

These are gallery tests for image wrapped in `<figure>` elements.

To place a gallery add the necessary YAML Front Matter, like we did above!

```yaml
gallery:
  - url: unsplash-gallery-image-1.jpg
    image_path: unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: unsplash-gallery-image-2.jpg
    image_path: unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: unsplash-gallery-image-3.jpg
    image_path: unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
    title: "Image 3 title caption"
  - url: unsplash-gallery-image-4.jpg
    image_path: unsplash-gallery-image-4-th.jpg
    alt: "placeholder image 4"
    title: "Image 4 title caption"
```

And then drop-in the gallery include --- gallery `caption` is optional.

```liquid
{% raw %}{% include gallery caption="This is a sample gallery with **Markdown support**." %}{% endraw %}
```

{% include gallery caption="This is a sample gallery with **Markdown support**." %}

This is some text after the gallery just to make sure that everything aligns properly.

The gallery below will be an example for gallery 2, in the YAML Front Matter.


```liquid
{% raw %}{% include gallery id="gallery2" caption="This is a second gallery example with images hosted externally." %}{% endraw %}
```

{% include gallery id="gallery2" caption="This is a second gallery example with images hosted externally." %}

An example for gallery3 is given below - You can name your gallery whatever you want, but make sure to replace the code with the same name.
As you can see, we have added `class = "Full"`, which means that it will occupy the entire container (screen).

{% include gallery id="gallery3" class="full" caption="This is a third gallery example with two images and fills the entire content container." %}