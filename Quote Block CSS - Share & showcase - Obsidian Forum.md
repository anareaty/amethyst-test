---
id: e2d7a371-c278-4540-89ce-c7bc5f8e081a
date: 2023-12-11
cssclasses:
  - saved
Источник: https://forum.obsidian.md/t/quote-block-css/4640
Тип: статья
Тема:
  - "[[Obsidian|Obsidian]]"
Раздел: "[[Сохранено]]"
Статус статьи:
  - 📑 проработать
---


I’m looking to restyle the CSS for quote blocks. For those of you who have changed it, how do your quote blocks look?

* [last reply6d](https://forum.obsidian.md/t/quote-block-css/4640/22)
* 8.2k  
#### views
* 13  
#### users
* 18  
#### likes
* 2  
#### links

[![block](https://proxy-prod.omnivore-image-cache.app/690x50,sUTNKl9NgIhXofQIh9MxPQNjmLiNb-mDfvAVmyD-cz7E/https://forum.obsidian.md/uploads/default/optimized/2X/4/45858100b9b3f257b43e93ee28e97901f18402d2_2_690x50.png)](https://forum.obsidian.md/uploads/default/original/2X/4/45858100b9b3f257b43e93ee28e97901f18402d2.png "block")

[![block2](https://proxy-prod.omnivore-image-cache.app/690x103,sl4zO7hwPbJjKrhsbgbmDZiB8pg4bwYNobGllOvGqumo/https://forum.obsidian.md/uploads/default/optimized/2X/a/a3a6a5bc6a3559c354be313214912456afea5e8d_2_690x103.png)](https://forum.obsidian.md/uploads/default/original/2X/a/a3a6a5bc6a3559c354be313214912456afea5e8d.png "block2")

Here’s mine fwiw  

[![image](https://proxy-prod.omnivore-image-cache.app/690x262,svBHqoEwWjJpd7qd8wX22SHsz_Seqh2HNNKA5w1gG-lE/https://forum.obsidian.md/uploads/default/optimized/2X/5/5dba61ca5e96fd5590a11ea160f56c5c2beb4c74_2_690x262.png)](https://forum.obsidian.md/uploads/default/original/2X/5/5dba61ca5e96fd5590a11ea160f56c5c2beb4c74.png "image")

I mostly use quotes as highlighters/alert boxes:  

[![image](https://proxy-prod.omnivore-image-cache.app/580x500,s-82bFn4K-wolxXoKTrQOZ68TyWYgJClQaUDs-pMzeFM/https://forum.obsidian.md/uploads/default/original/2X/a/a7be22d5a7c775ac156450c0465f2abe355bea4f.png)](https://forum.obsidian.md/uploads/default/original/2X/a/a7be22d5a7c775ac156450c0465f2abe355bea4f.png "image")

Could you be willing to share the snippet for your quote block. It looks intresting.

Can you please send me your css snippet for this style?

Can you send me your css snippet?

It is dark / light theme sensitive.

```scss
.markdown-preview-view blockquote {
    border-color: transparent;
    font-size: 95%;
    text-align: center;
    hyphens: auto;
    word-break: keep-all;
    color: var(--text-muted); # you need to define
    font-color: #aacdbe;
    line-height: 1.3;
    padding: 1px 2% 1px 2%;
    margin-top: 15pt;
    margin-bottom: 15pt;
}
```

Here you go… apologies or the delay. I no longer use this snippet for my quotes, so I had to reconstruct it. This snippet works in both edit and preview modes. It is probably a mess if you know anything about css (I know just enough to be dangerous):

```css
.cm-quote {
    color: var(--text-normal) !important;
}

.markdown-preview-view blockquote {
    background-color: transparent;
    border: 0px solid;
    border-color: rgb(126, 124, 124) !important;
    border-left-width: 8px !important;
    border-radius: 20px 8px 8px 20px;
    font-family: sans-serif;
    color: black; 
    font-size: 15px;
    font-style: italic;
    line-height: 1.5em;
    margin: 0 10px;
    padding-top: 12px;
    padding-bottom: 13px;
}

div:not(.CodeMirror-activeline)>.HyperMD-quote {
    background-color: transparent;
    border: 0px solid;
    border-color: rgb(126, 124, 124) !important;
    border-left-width: 8px !important;
    border-radius: 20px 8px 8px 20px;
    font-family: sans-serif;
    color: black; 
    font-size: 15px;
    font-style: italic;
    line-height: 1.5em;
    margin: 0 10px;
    padding-top: 12px;
    padding-bottom: 13px;
}

```

how can you different styles of blockquote?

we have callout now ([Use callouts 293](https://help.obsidian.md/How+to/Use+callouts)), easier to style that. in fact it has a number of presets already (including quotes) 

Great! That’s exactly what I want.

Could you share your CSS please? I’m having difficulties to edit the CSS code for blockquote as a whole, and set border-radius for the box and not line by line.  
Thanks!

You are referring to a 3-year old post!! I have changed themes many times since and my CSS has evolved with it. If you are interested I can share what I am using now.

I am interested as well [@Klaas](https://forum.obsidian.md/u/klaas)!

Are you in the Discord group?

Sorry for the late reply, I was away.  
I am using the Listive theme, without CSS snippets. I do have customized snippets for 13 different themes; if you are interested in any of those, let me know which one(s).


