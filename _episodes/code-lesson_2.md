---
title: Code Lesson
teaching: null
exercises: null
duration: null
summary: This template shows you how to include computer code and its output in
  your lessons.
questions: null
objectives: null
keypoints: null
is-break: null
ukrn_wb_rules:
  - allow-multiple
day: 1
order: 100000
missingDependencies: []
dependencies: []
originalRepository: UKRN-Open-Research/ukrn-wb-lesson-templates

---
## Markdown

### Code

Code blocks are written using triple backticks:
```markdown
    ```language
    code goes here
    ```
    {: .section-tag}
```

These sections can be styled according to what they're supposed to present.

```javascript
console.log("We use the {: .source} tag to show code that people can write.")
```
{: .source}

```
> "We use the {: .output} tag to show expected output."
```
{: .output}

```
> "We use the {: .warning} tag to show a warning message."
```
{: .warning}

```
> "We use the {: .error} tag to show errors."
```
{: .error}

### Advanced Code Tags

You can nest code tags within other tags:

```markdown
> ## Question
> Currently we have a line of code that produces an error:
> ```javascript
> const hello = ["hello", "world"];
> console.log(hello.combine(', '))
> ```
> {: .source}
> ```
> > Uncaught TypeError: hello.combine is not a function
> ```
> {: .error}
> How can we fix this to write `hello, world` to the console?
>
> > ## Solution
> > We need to use the appropriate method. The `Array` prototype [has a `join` method](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join) that does what we need:
> > ```javascript
> > const hello = ["hello", "world"];
> > console.log(hello.join(', '))
> > ```
> > {: .source}
> >
> > ```
> > > "hello, world"
> > ```
> > {: .output}
> {: .solution}
{: .challenge}
```

> ## Question
> Currently we have a line of code that produces an error:
> ```javascript
> const hello = ["hello", "world"];
> console.log(hello.combine(', '))
> ```
> {: .source}
> ```
> > Uncaught TypeError: hello.combine is not a function
> ```
> {: .error}
> How can we fix this to write `hello, world` to the console?
>
> > ## Solution
> > We need to use the appropriate method. The `Array` prototype [has a `join` method](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join) that does what we need:
> > ```javascript
> > const hello = ["hello", "world"];
> > console.log(hello.join(', '))
> > ```
> > {: .source}
> >
> > ```
> > > "hello, world"
> > ```
> > {: .output}
> {: .solution}
{: .challenge}
