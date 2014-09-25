# Crash Course on CSS

Yeah... look through stuff... try it out... make it pretty.

YOU CAN DO IT.

## Structuring your HTML
- Basic Layout (Part 1 & Part 2)

## CSS Examples


## Advanced CSS Examples
- Post Tags
- Off Canvas Menu

## CSS Preprocessors (ex: LESS & SASS)

### What is a CSS preprocessor?
[Wikipedia article on preprocessors](http://en.wikipedia.org/wiki/Preprocessor)

A CSS preprocessor is essentially a supercharged version of CSS that has more functionality
like mixins (functions), variables, nesting, and inheritance.

Imagine being able to change a single color variable and have your entire site
change almost instantly. Immediate color scheme change without having to go out
and change each and every place where you are using that specified color.

SASS and LESS are the two primary preprocessors, but there are many others.
Which one you choose is really up to your own preference.

If you want to see what I mean by that, I encourage you to go through these:
[LESS Features](http://lesscss.org/features/)  
[SASS Guide](http://sass-lang.com/guide)

### [LESS](lesscss.org) Workflow
#### Important Note for ALL listed workflows
It is good to have one centralized LESS file that has all of the other files imported
into it. All other files should be named ```*.import.less```.

So, you have one file ```style.less``` that has everything in it.
```less
@import 'variables.import.less';
@import 'mixins.import.less';
@import 'base.import.less';
@import 'home.import.less';
@import 'blog.import.less';
```
The reason that it should be this way is so that you can structure the way your CSS outputs.
The order that CSS is in really does matter. Styles that are instantiated later take precedence
and can override similar styles from before.

And this is the file that is compiled to CSS at the end. 

#### With Gulp


#### With Meteor
Add in the LESS package
```meteor add less```

## Using Design Frameworks
You always want to be able to follow the [DRY](http://en.wikipedia.org/wiki/Don't_repeat_yourself) principles.
So, why re-do CSS when you can utilize a framework and speed up your design process. Focus on the
nicer pieces of your website and what make it unique. Avoid spending time on the base
css that can be repeated and improved project after project.

There are three primary CSS design frameworks:  
[Bootstrap](getbootstrap.com) - Most Popular  
[Foundation](foundation.zurb.com)  
[Semantic-UI](semantic-ui.com) - Newer, but very nice  
