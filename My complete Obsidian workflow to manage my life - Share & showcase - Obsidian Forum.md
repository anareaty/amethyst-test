---
id: 25421879-8a3b-4f94-a167-82c10b693aaa
date: 2023-12-11
cssclasses:
  - saved
Источник: https://forum.obsidian.md/t/my-complete-obsidian-workflow-to-manage-my-life/64522/3
Тип: статья
Тема:
  - "[[Obsidian|Obsidian]]"
Раздел: "[[Сохранено]]"
Статус статьи:
  - 📖 прочитать
---


## [](My%2520complete%2520Obsidian%2520workflow%2520to%2520manage%2520my%2520life%2520-%2520Share%2520&%2520showcase%2520-%2520Obsidian%2520Forum.md##introduction-1)Introduction

[![image](https://proxy-prod.omnivore-image-cache.app/690x431,s9JpBh2aqU7wVlmEl1GPEypwl_ZjEBtmBKURiYl5OHz0/https://forum.obsidian.md/uploads/default/optimized/3X/4/b/4b959daec192357b817010d63fec0222ad57fa3a_2_690x431.jpeg)](https://forum.obsidian.md/uploads/default/original/3X/4/b/4b959daec192357b817010d63fec0222ad57fa3a.jpeg "image")

As I promised to quite a few people on different places, I’m releasing a full blown guide of my Obsidian workflow. It has many cool features that I’ve seen people struggling with online :

1. Tasks and project management with journaling, workout logging and media tracking. Using daily and periodic notes.
2. Read-it-later with automated conversion to markdown and import inside your vault. Meaning all your past knowledge is inside Obsidian, available with a simple search alongside your notes.
3. Fast and simple one click upload obsidian publish alternative.

But there’s plenty more. It took me some time here and there during the past year to come up with this setup. And don’t worry, it is **easy to use** despite its awfully long name. But I’ll describe it with as much depth as I can for people who wants to fine tune it.

Obviously, it is merely just a starting point, with Obsidian you can (and you always should) do something that works well for **you**. And that means creating your **own** setup. But that doesn’t forbid you from using this one as a starting-point.

Links :

* [My Complete Obsidian Workflow to Manage My Life 166](https://mathisgauthey.github.io/my-complete-obsidian-workflow-to-manage-my-life/)
* [Why Using Obsidian for Life Management 45](https://mathisgauthey.github.io/why-using-obsidian-for-life-management/)
* [Obsidian Publish Alternative, How to One-click Upload Your Notes on Your Own Website 32](https://mathisgauthey.github.io/obsidian-publish-alternative-how-to-one-click-upload-your-notes-on-your-own-website/)
* [A template vault available on Github to try it for yourself 72](https://github.com/mathisgauthey/obsidian-workflow-template)

## [](My%2520complete%2520Obsidian%2520workflow%2520to%2520manage%2520my%2520life%2520-%2520Share%2520&%2520showcase%2520-%2520Obsidian%2520Forum.md##core-features-2)Core Features

* Beautiful design using [AnuPpuccin: Personal theme for Obsidian 47](https://github.com/AnubisNekhet/anuppuccin).
* [P.A.R.A 36](https://fortelabs.com/blog/para/)\[^1\] folder organisation based on file actionability.
* [GTD 16](https://gettingthingsdone.com/)\[^2\] task management on par with a [full Todoist setup 16](https://todoist.com/fr/productivity-methods/getting-things-done), but with a simple and natural way of **writing tasks alongside notes**. You also get to keep your project tasks, notes and files archives when you finish a project, allowing you to access these informations in the future.
* Daily notes for task management, periodic notes for projects management (week, month, quarter and year).
* Journal section for each daily and periodic notes to write about anything that happened during a certain period of time.
* Simple workout log for storing your workout sessions but with an infinite possible personalized exercise library.
* Media backlog Kanban board for tracking books, shows, movies or video games backlog, consuming media at the right pace, and archiving what you do. All without proprietary online services that hold you data.
* Read-it-later / bookmark manager with automated markdown conversion for offline storage inside your vault using [Omnivore app 29](https://omnivore.app/). That means easy search for knowledge inside your vault across sources and personal notes.
* [Zettelkasten note-taking 9](https://everlaab.com/methode-zettelkasten-comment-prendre-des-notes-utiles/) on a flat structure inside `3-Resources` folder.  
   1. Import sources automatically using [obsidian-omnivore 8](https://github.com/omnivore-app/obsidian-omnivore) plugin for an automatic markdown conversion of a webpage or document online or manually from a file or using [markdownload 3](https://github.com/deathau/markdownload).  
   2. Highlight and take reference notes using [Omnivore app 29](https://omnivore.app/) or directly inside your vault using a simple markdown file.  
   3. Write literature notes to summarise the source informations.  
   4. Write permanent notes from key concepts directly inside literature notes using wiki-links.
* One click upload of file and attachments to a [Hugo 9](https://gohugo.io/) website hosted on [Github Pages 2](https://pages.github.com/) thanks to [obsidian-github-publisher 8](https://github.com/ObsidianPublisher/obsidian-github-publisher) plugin.

* [last reply](https://forum.obsidian.md/t/my-complete-obsidian-workflow-to-manage-my-life/64522/5)
* 1.9k  
#### views
* 2  
#### users
* 15  
#### likes
* 16  
#### links

Hello [@RedeyeFR](https://forum.obsidian.md/u/redeyefr) and thanks for sharing! I’m very interested in your workflow as I’m trying to set up a very similar one for tasks; I’m especially interested in your todoist/obsidian tasks plugin approach. If I understand correctly you jot down your tasks on the way in todoist and then how do you transform in obsidian tasks? Or am I wrong?  
Thanks for any advice !

Hi there ! Yup, I’m using todoist as a quick way to input things I don’t want to forget.

Then during the day I go on my daily note which has a todoist code block thanks to the obsidian-todoist plugin and I can see my inbox. From there I used to copy these task manually by selecting them and creating various stuff (tasks, projects, notes, etc).

But right now I have quite a more… Complete approach ? I’m using the quickadd plugin and a [script 8](https://quickadd.obsidian.guide/docs/Examples/Capture%5FFetchTasksFromTodoist) that allows me to automatically import all of these inside my vault.

I did not and still do not have time to update the template workflow but I made some significant improvement over the last few months based on reviews and on my personal usage that grew. But one day… 

Wow [@RedeyeFR](https://forum.obsidian.md/u/redeyefr), it worked like a charm!!! And it’s perfect for my workflow. Just one thing I’d like to keep, in some cases, the tasks in Todoist and tried to see the code to remove the function call to `closeSelectedtask` but as I have no experience with js script I don’t know which part of the script I have to cut off (there’re three lines where it appears, I think…)  
merci beaucoup 

Hey there, glad it helped ! You can copy and paste another script that you’ll use, remove all `closeSelectedTasks` function calls and it should be alright I guess.


