1. Describe the most difficult/painful hurdle you had to overcome in implementing your solution.

Nothing really. It was quite easy. I had everything working and tested along with documentation in half an hour.

2. Describe which puppet related concept you think is the hardest for new users to grasp.

For me it would be the declarative vs. imperative form. You have to keep track of the precedence and dependencies.

2. Describe which puppet related concept you think is the hardest for new users to grasp.

Idempotence is one of the core characteristics of all modern configuration management tools. Without it, it's like old bash days. Running something twice could cause a lot of headache.

4. Where did you go to find information to help you in the build process?

I copied the Vagrantfile from [the template](https://github.com/navidpaya/dotfiles/blob/master/Vagrantfile) I keep in my own repo. For the Ansible code, I mostly consulted the [Ansible documentation](http://docs.ansible.com/) which is pretty good. A few clean runs on the vagrant box and all was good to go.

5. In a couple paragraphs explain what automation means to you and why it is important to an organization's infrastructure design strategy.

To me automation is the whole difference between what I used to do as a pure sysadmin (most of which I hate except for the hands on which is an essential) and what I do nowadasy which is just writing code to make sure things are set up automatically and zerop assumptions. It is what makes the developers not come to me with the same problme every single days because I really hate things repeating myself. It is what changes the way you look at your servers (cattle vs kittens). It enables you to look at almost everything in your infrastructure as disposable resources (although I've come to think we're under illusion of making things stateless while all we're doing is moving states from everything else to our databases and making them single points of failure but still better than how things used to be). It makese it possible to reapeat, test and verify everything related to infrastructure and toolings. It makes it possible to get code from the developer to production much more efficiently.