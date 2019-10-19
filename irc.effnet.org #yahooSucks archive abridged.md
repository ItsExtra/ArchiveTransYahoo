# Selective archive of irc.effnet.org #yahooSucks

For my own records 

Anyone can join here: http://chat.efnet.org:9090/?%23yahoosucks 

Saturday October 19, 2019 191019

[17:42] <Solanum> hello

[17:42] <Solanum> I was about a week into learning about this archiving stuff when this yahoo groups thing happened

[17:43] <Solanum> I am a trans man (aka FTM) and a lot of our history is on those groups

[17:43] <Solanum> they were very very important

[17:43] <Solanum> I am abit panicked trying to learn fast which doens't work

[17:45] <Solanum> All these groups are set to private

[17:45] <Solanum> Is there a page somewhere that you can reccomend me to read?

[17:45] <@betamax> Solanum: hi! thanks for stopping by

[17:46] <@betamax> by "private" do you mean that all new membership requests must be approved by an admin?

[17:46] <Solanum> Yes

[17:46] <Solanum> And some of them are inactive x years

[17:46] <Solanum> So it'll be a lot of work jsut to get into them

[17:46] <Solanum> But it's probably doable

[17:46] <@betamax> OK. Are you a member of all the groups you want to archive?

[17:46] <Solanum> Nope!

[17:47] <@betamax> right. That could be difficult.

[17:47] <Solanum> It's s mall community

[17:47] <Solanum> If I bother enough people I should be able to get in to at least some of them

[17:47] <@betamax> I would recommend trying to join them, then asking around to see if someone has already joined

[17:48] <@betamax> because it isn't strictly necessary for you to be a member, only that you can borrow the Yahoo account of someone who is

[17:48] <Solanum> Once I do that, is there a way to get the data? I was tryign to follow the chat above and it looks.. not straight forward

[17:48] <Solanum> hmm good point. they would need to trust me

[17:49] <@betamax> "chaotic fast development due to impending yahoocalypse" was one description of the work on the archival scripts right now

[17:49] <Solanum> OK maybe I'll give that a bit of time and work on getting access

[17:49] <Solanum> I have started a list https://calc.disroot.org/tijh1mt2c7v7

[17:50] <@betamax> basically, there are many tools to get just messages, and we're (or,  rather nico_32_ is) standardising on one tool to get everything from a  group

[17:50] <Solanum> I don't even know the names of all the groups. They are not a big thing now. But 10-20 years go.

[17:50] <@betamax> yes, access is the main thing

[17:50] <Solanum> Other than mesages what is there?

[17:50] <@betamax> photos / files / attachments / events / polls / links

[17:50] <Solanum> Right. Off course. 

[17:51] <Solanum> I will also need to convince people I am trustworthy. The groups are  private for ar eason, whcih is that people put very, very intimate  details fo their lives in them. 

[17:51] <Solanum> Like there are groups about genital surgery etc

[17:52] <@betamax> it is for that reason that "private" groups aren't going to be archived by us (archiveteam), although we will point you towards tools to do it  yourself

[17:52] <Solanum> Yes that's reasonable

[17:52] <@betamax> Yahoo are starting the first step towards closure on the 28th when they stop adding new content to the site

[17:52] <@betamax> there is a danger that at this point they no longer allow people to sign up to groups

[17:53] <@betamax> (the plan is for everything to eventually be invite-only)

[17:53] <Solanum> Yes I thoiught of that. i didn't know if it meant that or not. 

[17:53] <@betamax> so I would recommend getting access to all the groups you want to save by 28th Oct

[17:53] <@betamax> It's Yahoo... we're assuming the worst (although they did change it from the 21st to 28th, which is good)

[17:54] <Solanum> By the way if anyone else interested in LGBTQIAetcetc shows up, I can be reached at inthere@disroot.org 

[17:54] <Solanum> I am going to write something to send around to start on that. I wanted to know what there was by way of a plan for actually getting the data  before i started. Sounds like that is TBD at the moment

[17:55] <Solanum> Is this the best place to find updates or is there somewhere easier to catch up on?

[17:55] <@betamax> so, there is a script that can get everything (except maybe polls)

[17:55] <@betamax> but it is very flakey

[17:55] <Solanum> Can any member use it?

[17:55] <@betamax> yes, we'll have a solution at some point, hopefully mid-week at the latest

[17:56] <@betamax> https://github.com/nsapa/yahoo-group-archiver

[17:56] <@betamax> that's it there

[17:56] <Solanum> What about something like site-sucker or grab-site or wget?

[17:56] <@betamax> more difficult, as you'll need to deal with cookies and JS

[17:56] <Solanum> Those were the ones I was working on learning before I found out about this

[17:56] <Solanum> So they won't work really at all?

[17:57] <Solanum> Or will work but not ideally?

[17:57] <@betamax> they'll work for public groups, but not (without tweaking) for private groups

[17:57] <Solanum> because you need to be logged in?

[17:58] <@betamax> yes, and because some things on the site use javascript to load, which those other tools don't work as well on

[17:58] <Solanum> oh gosh

[17:59] <Solanum> I read something about using a cookies.txt file for logins for wget (or mabe grab-site) but if there is javascript for showing content.. that's a problem

[18:00] <@betamax> there may not be for messages, but I think things like images might not work as well

[18:01] <@betamax> hence the work on specialist tools just for Yahoo Groups

[18:01] <@betamax> we'll be releasing instructions on how to use the tools once they're ready

[18:01] <Solanum> I think getting anything would be better than nothing, but for the  groups I am hoping to get images are a huge component. People putt heir  surgery pics and other stuff like that. 

[18:02] <Solanum> I should watch the github linked above for thaT?

[18:03] <teovall> yes, momentum seems to be converging on that script... so that repo or  one of it's forks is likely to be the tool of choice going forward

[18:04] <Solanum> OK great

[18:04] <teovall> i'd say it's at the 80% point... 80-90% should go quick... it's that last 10% that will tough

[18:04] <Solanum> In the event that any of these groups are public, is there a list of  what has already been archived, or what is in the queue, so I don't have to spend time duplicating work?

[18:05] <@betamax> the best place to check is probably the wiki

[18:05] <Solanum> Ya there is usuallya. reason to leave certain bits til the end.. that they are extra difficult haha

[18:05] <@betamax> as we'll link to a tool and have instructions there once done

[18:06] <Solanum> this? https://www.archiveteam.org/index.php?title=Yahoo!_Groups

[18:06] <@betamax> tes

[18:06] <@betamax> *yes

[18:06] <Solanum> perfect thank you so much for taking your time

[18:06] <Solanum> <3

[18:06] <@betamax> if you find public groups, or ones that don't need member approval

[18:06] <@betamax> then we have a nomination form

[18:06] <@betamax> https://tinyurl.com/savegroups

[18:07] <@betamax> although if you want to be safe, archive it yourself as well

[18:07] <Solanum> OK noted