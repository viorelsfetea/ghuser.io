> Work in progress

<p align="center">
  <a href="https://ghuser.io">
    <img src="https://rawgit.com/AurelienLourot/ghuser.io/master/docs/logo.png"
         width="400" height="108" />
  </a>
</p>
<p align="center">
  <b>Better GitHub profiles</b>
</p>
<br />

# What we are building

We love the default GitHub profiles and we want to enhance them:

* The GitHub profiles aren't clearly showing all repos you have contributed to since you joined
  GitHub. We are showing them **all**, even those you don't own and aren't affiliated to in any
  way.<sup>[1](#footnote1)</sup>
* The GitHub profiles are listing all the repos you own but they sort them only by age of the
  latest commit. We prefer to **sort repos** by a combination of how active they are, how much you
  have contributed to them, how popular they are, etc. For each user we want to see first the latest
  greatest repos they have most contributed to.
* On GitHub only repos earn stars. We push it one step further by tranfering these **stars to
  users**. If you have built 23% of a 145 stars repo, you deserve 33 stars for that contribution. We
  add all these stars and clearly show how many of them you earned in
  total.<sup>[2](#footnote2)</sup>
* The GitHub profiles don't clearly show how big your contribution to a repo was, when you don't own
  it. Maybe you wrote 5%. Maybe 90%. We **make it clear**.
* GitHub detects programming languages. We want to also know about **technologies/frameworks**, e.g.
  "react", "docker", etc.<sup>[3](#footnote3)</sup>
* The GitHub profiles allow filtering your repos by programming language. We will allow **filtering
  by technologies/frameworks** as well.
* The GitHub profiles can be tweaked by clicking around. We allow them to be **tweaked
  programmatically**.<sup>[4](#footnote4)</sup>
* On GitHub only users and organizations have avatars. We bring
  [**avatars to repos**](docs/repo-settings.md).

Our enhanced profiles are accessible at `https://ghuser.io/<github-username>`, e.g.
[ghuser.io/AurelienLourot](https://ghuser.io/AurelienLourot).

<a name="footnote1"><sup>1</sup></a> We achieve this by using [github-contribs](https://github.com/AurelienLourot/github-contribs).<br/>
<a name="footnote2"><sup>2</sup></a> This will be implemented by [#4](https://github.com/AurelienLourot/ghuser.io/issues/4).<br/>
<a name="footnote3"><sup>3</sup></a> This will be implemented by [#9](https://github.com/AurelienLourot/ghuser.io/issues/9).<br/>
<a name="footnote4"><sup>4</sup></a> This will be implemented by [#12](https://github.com/AurelienLourot/ghuser.io/issues/12).

# Get your profile!

We are still building the [first prototype](https://github.com/AurelienLourot/ghuser.io/milestone/1)
but you can already be an early user and get your profile by
[creating an issue](https://github.com/AurelienLourot/ghuser.io/issues) :)

# Build and run locally

[ghuser.io](https://ghuser.io) is a [Reframe](https://github.com/reframejs/reframe) web app:

```bash
$ cd reframe/
$ npm install
$ npm run local
...
 ✔ Server running (for development)
     http://localhost:3000/ -> LandingPage
     http://localhost:3000/:username -> ProfilePage
     http://localhost:3000/logo -> LogoPage
```
