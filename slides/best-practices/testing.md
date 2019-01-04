## Test Your Code

Note: We've  found that adding unit tests to the widgets you're developing pays huge divedends towards having a higher quality and lower maintainance code base.

The obvious benefit is a reduction in regressions as your widget grows in scope.  If you add a test every time a new bug is found or feature added, the chances that bug will pop up again on deployment is greatly reduced.

That being said, the largest benefit for me since I've made test driven development a habit doesn't come from running the tests themselves, but as a design aide.  Writing tests forces you to write easily testable code.  Easily testable code tends to be cleaner, more user focused, and generally less like a giant pile of spaghetti.

I know what you're thinking.  This sounds great and I know I should start implementing more tests...

---

### ...but its hard, and I don't have time

* Write tests before features <!-- .element: class="fragment" -->

* Estimate test writing as part of your design process <!-- .element: class="fragment" -->

* Start small <!-- .element: class="fragment" -->

* Only test your code <!-- .element: class="fragment" -->

Note: Maybe you'll start walking around the last day of this conference with the intention of writing unit tests for your entire code base and pushing your team to do the same, but you might also get back to the realities of work (deliverables, budget, reluctant team members) and push it off as one more thing that you should get to if I find the time...  It doesn't have to be like that, make writing tests easy and developers will write them.  If writing tests is hard, they won't, no matter how grand your vision of a perfect code base is.  So, how do we make writing tests easy for Web App Builder?

Like I mentioned before, if you write tests around user requirements or bug descriptions, there's a tendency to write testable code.  Developers are really good and writing code that's really hard to test, so write the tests first.

The time dellema is one I see come up constantly.  We already estimated this feature and didn't include tests in there.  Our clients won't give us the budget for writing tests. If you include designing features in your estimates, you should also include tests.  As you design your new features, or troubleshoot the source of a bug, start writing your test.  It will end up being more user centered, and likely save time in development over the course of the feature.

Start small. Don't go and try to redesign your entire code base for complete coverage.  Pick small features and add tests a little bit at a time.  That way, you don't end up with a massive task that keeps getting pushed off for other priorities.  Or, don't add any tests for existing code and features.  Incorporate tests into your design process and start adding tests for every new feature and bug.  Your coverage percentage will naturally increase, your code quality will improve with it, and you won't be adding any additional tasks to your project.

Finally, if you ever talk to me about unit testing, you'll here me drive home this point again and again.  Only test YOUR code.  The Web App Builder and JavaScript API have their own development teams.  It's their job to write tests for their code, not yours.  Write tests to make sure you're testing only the code you've written.  This generally means abstracting away dependencies and mocking JavaScript API classes or functions.  How do we abstract the Web App Builder away from Web App Builder Widgets?

