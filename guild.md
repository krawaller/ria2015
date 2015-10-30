###Purpose of the Guild

The [guild](http://blog.krawaller.se/riaguild2015) is a list of all course participants, with links to their projects, blog posts and pull requests. This is to allow us to more easily snoop on what the others are up to!

There is no communication channel on the guild; that is taken care of through the [course Slack channel](../slack). The guild is **only** for static content.

###Joining the guild

To enter your data into the guild you must go to the [git repo](https://github.com/krawaller/riaguild2015) and **fork** it. In your fork you must add a JSON file describing yourself into the `src/data/users` folder. Please use your **github** username as ID. For example, my github name is `krawaller`, so my file is at `src/data/users/krawaller.json`.

Here is what my file looks like:

```javascript
{
	"name": "David Waller",
	"github": "krawaller",
	"projectrepo": "riastart2015",
	"projectdesc": "Super hero battler 2000! A small demo of React+Redux+Router.",
	"slack": "david.waller",
	"presentation": "36 year old Ystad resident, long time JavaScript lover. Heading up this course!",
	"icon": "human-magi$elder-mage",
	"blogposts": [
		{
			"when": "2015-10-29 20:30",
			"url": "https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/",
			"title": "Course page"
		}
	],
	"pullrequests": [
	]
}
```

Please format yours to contain the same keys! To begin with you can omit `projectrepo` and `projectdesc` as you don't have that up and running yet. Likewise the `pullrequests` array will be empty (although still included), but the `blogposts` array should contain an entry for your first post, as per the initial course step instruction.

After you have added your JSON file you must also make sure it is read into the main data by editing `src/data/members.js`. Here's what it looks like right now, with me as the sole member:

```javascript
module.exports = {
	krawaller: require("./users/krawaller.json")
};
```

Again, please use your github user name as key for the entry.

###During the course

Throughout the course you should update your JSON file whenever you write a new blog post, or have made a pull request on a classmate (instructions on syntax forthcoming). This is important - if you only announce your post/PR on Slack I might miss it, and if I haven't seen it, it hasn't happened! 

Also - as you have no doubt noticed, the guild is really rather drab-looking. Feel super free to make pull requests to spice it up!
