## Student Projects

A list of open source projects that students can contribute to for student projects. Please feel free to join an existing project and collaborate. All your contributions to any project you've collaborated on will count toward your student achievements.

Do you have a project idea? [Please share!](https://github.com/learn-javascript-courses/student-projects/issues/new?title=Project+idea)

### [Rejection](https://github.com/learn-javascript-courses/rejection) #basic #intermediate #advanced

The game where you have to lose to win! Train yourself to be a better negotiator and win at life by asking for more and learning to appreciate rejection.

### [Let's Hangout](https://github.com/learn-javascript-courses/lets-hangout) #basic #intermediate #advanced

Bored? Want to hang out with friends, but not sure who's available? This app will connect to your favorite social network and allow you to post a hangout invitation status message. It will also collect recent status updates from all your friends looking for similar invitations, and will watch for replies to your status message so you can see who else wants to hang out right now. Once you've selected who you want to hang out with, you can post an event update with a time and place to meet.

### [CheckIn](https://github.com/learn-javascript-courses/checkin) #intermediate

A simple scrum helper app to keep track of what people on your teams are working on, without the scrum meeting.


### rtype

#### [Runtime rtype parser](https://github.com/ericelliott/rtype/issues/62) #advanced

You'll learn about how programming language compilers parse source code, extract its meaning, and compile output from it.

Write a function that takes an rtype interface description as a string and returns an object that can be used for runtime type checking.

```js
interface TypeChecker {
  checkInputs: Predicate,
  checkOutput: Predicate,
  checkError: Predicate
}

parseSignature(signature: String) => TypeChecker
```

The target function will get wrapped by a utility such as [rfx](https://github.com/ericelliott/rfx). When the wrapper function gets called, it will pass inputs to `checkInputs()`. If it returns true, only then does the original function get called. When the function returns, its output will be similarly checked by `checkOutput()` before it gets returned to the original caller. If the function throws, the error will also be checked, by `checkError()`.

Useful background:

* [How to Build a Compiler](https://www.youtube.com/watch?v=Tar4WgAfMr4) Great video by James Kyle
* [How to Build a Compiler source](https://github.com/thejameskyle/the-super-tiny-compiler) Source companion to the James Kyle video
* The [Stanford Compilers course](https://www.coursera.org/course/compilers) (free online lectures)

If you're curious about types, see the [introduction to types](https://class.coursera.org/compilers/lecture/45) from the Stanford Compiler course.
