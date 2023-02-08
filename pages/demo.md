---
title: Writing Features Demo
layout: essay
permalink: /demo.html
---


## Images 


### Image the size of the text block


```{% raw %}{% include essay/figure.html objectid="im-06" %}{% endraw %} ```

{% include essay/figure.html objectid="im-06" %}

### Full page wide image

```{% raw %}{% include essay/figure-full-page.html objectid="im-06" %}{% endraw %}```

{% include essay/figure-full-page.html objectid="im-01" %}


## Margin note 

### Example

This is a fake paragraph so that we can demonstrate the margin note. 
{% include essay/marginnote.html id="marginnote-3" text="This is a margin note that is linked to the end of the sentence or even placed in the middle of a sentence." %} The margin note is a note that goes in the margin, so it is well named. 

```{% raw %}{% include essay/marginnote.html id="marginnote-3" text="This is a margin note that is linked to the end of the sentence or even placed in the middle of a sentence. Note that nothing connects to the text (there is no marker) but if you are on a phone, a little bullseye thing shows up."%}{% endraw %} ```

### Options:

- "text" = text for the margin note -- this can be written in HTML to add links, etc. 
- "id" = a unique id (short phrase is best) to connect the location and note
- "text-link" = [optional] link for the entire note; you can also add links to certain words via writing the text in HTML
- "color" = [optional] a Bootstrap color (primary, secondary, success, danger, warning, info, light, dark)


## Margin Note with Image 


### Example

Habitasse platea dictumst quisque sagittis purus sit. Quam elementum pulvinar etiam non. Faucibus scelerisque eleifend donec pretium vulputate sapien. Accumsan tortor posuere ac ut consequat semper viverra. Fringilla ut morbi tincidunt augue. {% include essay/marginnote-image.html id="tellus-note" text="This is a margin note with an image!." image="im-06"%}

``` {% raw %} 
{% include essay/marginnote-image.html id="tellus-note" text="This is a margin note with and image!." image="im-06"%}{% endraw %}```


### Options:

- "text" = text for the margin note -- this can be written in HTML to add links, etc. 
- "id" = a unique id (short phrase is best) to connect the location and note
- "text-link" = [optional] link for the entire note; you can also add links to certain words via writing the text in HTML
- "color" = [optional] a Bootstrap color (primary, secondary, success, danger, warning, info, light, dark)


## Sidenote 


### Example


```{% raw %}{% include essay/sidenote.html id="note2" text="This is a sidenote that is linked to the end of the sentence ending turips over there."%}{% endraw %} ```

This is a fake paragraph so that we can demonstrate the side note. 
{% include essay/sidenote.html id="note2" text="This is a sidenote that is linked to the end of the sentence ending turips over there."%} The sidenote is a note that goes on the side, so it is well named. 



### Options:

- "text" = text for the side note -- this can be written in HTML to add links, etc. 
- "id" = a unique id (short phrase is best) to connect the location and note
- "text-link" = [optional] link for the entire note; you can also add links to certain words via writing the text in HTML
- "color" = [optional] a Bootstrap color (primary, secondary, success, danger, warning, info, light, dark)


## YouTube Clip 


``` {% raw %}{% include essay/youtube-clip.html objectid="Spruce-grouse-takes-off" start="034" end="46"%}{% endraw %}```

{% include essay/youtube-clip.html objectid="Spruce-grouse-takes-off" start="034" end="46"%}


### Options:

- "objectid" = The objectid of the object you'd like to feature . This is the last bit of the url for that item, minus the ".html"
- "start" = second at which the clip starts
- "end" = second at which the clip ends


## Quotes

There are three levels of quote to use, and examples are below. 


### Examples

#### quote.html

{% include essay/quote.html text="Our last day in camp. The order to get ready for an early start tomorrow has gone forth, and we must leave our delightful wild life and return to the land of boiled shirts and stovepipe hats." objectid="cda_tpa1914" source="Page 28"%}


*Code for regular quote:* 

```{% raw %}{% include essay/quote.html text="Our last day in camp. The order to get ready for an early start tomorrow has gone forth, and we must leave our delightful wild life and return to the land of boiled shirts and stovepipe hats." objectid="cda_tpa1914" source="Page 28"%}{% endraw %} ```

#### quote-medium.html

{% include essay/quote-medium.html text="Rhythm is a recurring movement of notes and rests (silences) in time. It’s the human perception of time." source="iconcollective.edu" source-link="https://iconcollective.edu/basic-music-theory/"  align="right" color="info" %}

*Code for medium quote:* 

```{% raw %}{% include essay/quote-medium.html text="Rhythm is a recurring movement of notes and rests (silences) in time. It’s the human perception of time." source="iconcollective.edu" source-link="https://iconcollective.edu/basic-music-theory/"  align="right" color="info" %}{% endraw %} ```

#### quote-big.html

{% include essay/quote-big.html text="Rhythm is a recurring movement of notes and rests (silences) in time. It’s the human perception of time." source="iconcollective.edu" source-link="https://iconcollective.edu/basic-music-theory/"  align="right" color="info" %}


*Code for big quote:* 

```{% raw %}{% include essay/quote-big.html text="Rhythm is a recurring movement of notes and rests (silences) in time. It’s the human perception of time." source="iconcollective.edu" source-link="https://iconcollective.edu/basic-music-theory/"  align="right" color="info" %}{% endraw %} ```


### Options:

- "text" = text from the quote or source
- "source" = [optional] who said the quote / where the quoted text is coming from 
- "source-link" = [optional]  link to the source (center, right, left)
- "color" = [optional] a Bootstrap color (primary, secondary, success, danger, warning, info, light, dark)
- "align" = [optional] text alignment (center, right, left)

