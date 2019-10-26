###### 

There have been questions about the possibility of downloading the content of Yahoo Groups in such a way that they have identifying information removed.

It is important for me to say that I am not a programer, an expert in network security, or anything of the sort. The below is based on a general understanding of things to describe the difficulty of the problem to those who think it might be simple. 

# Why remove or redact information

The Internet Archive [team](https://www.archiveteam.org/index.php?title=Yahoo!_Groups) who are working on [the tools](https://github.com/IgnoredAmbience/yahoo-group-archiver/network/members) to "scrape" (download) the contents of the Yahoo Groups site to archive them have expended considerable effort to keep every detail about the messages and other Groups content. Since they are producing tools to download public, open groups, it makes sense to keep all available information

# What *can* be done

## Strip headers

Every email contains a chunk of information called "headers" which is used by computers and networks, but mostly hidden from users. Some headers which you will be familiar with are *To:*, *From:*, *Date:* and *Subject:*. Depending on how it's put together, there are lots of other bits of data. Here are some links if you'd like to learn more:

- [How to obtain email headers](https://support.google.com/mail/answer/29436?hl=en) in a variety of webmail providers and mail clients
- [Understanding an email header](https://mediatemple.net/community/products/dv/204643950/understanding-an-email-header) describes some of the basics of how to decipher email headers
- [Email Header Analysis](https://www.iptrackeronline.com/email-header-analysis.php) an automated tool that lets you copy and paste email headers form your own email to see *some* of the information available. A skilled, motivated investigator would likely be able to find more information than this tool will display. 

What you need to know is that these can be removed. It is not too difficult. It would not be desirable to remove all headers. For example, you would probably want to keep Subject, Date, and some other headers that make threads display correctly. Otherwise it would be confusing to read. Careful consideration by someone who understands the material would be ideal. 

In a situation where maximum preservation is desired, no headers would be removed whatsoever. 

## Remove correctly formatted email addresses

Outside of headers, it would not be difficult to write a script that would look for anything like *user@host.com* replace it with *[redacted]* or something else. However, if an address was entered differently, for example if spaces were introduced such as by typing *user @ host.com*, this would probably be missed. 

## Remove most names, and some other things

Slightly more complicated would be to remove names. This would never be perfect. However you could write a script that took all the names in the *From* header and searched for them in the rest of the body and replaced them with [redacted]. 

So if someone's *From* header is "Kayleb McCurdy," the script could search for "Kaleb" and "McCurdy" and redact them. Easy enough. But what if someone's *From* name was "Hope Red"? Would you want every use of the word "hope" and "red" to be removed? Or someone who's *From:* name is "ArchiveTransY" (like mine)? 

Some names that as also common English: Mark, Patience, Iris, Sage, Destiny, Liberty, Joy, Willy, Karma, Black, Green, White, Brown, Grey, Love, House, Small. Removing all such words would significantly impair the quality of the information, but it could be done. 







## Removal or sorting of photos and other images

Many mailing lists about surgery and other physical transition details were host to photos of the members, their bodies, etc. There are three strategies that can be employed:

1. Destroy all images (don't download them at all-- makes things much easier)
2. Keep all images
3. Destroy some images and keep others

The first two are simple. What of the third?

### Manual editing

Groups with a low volume of images and/or a large pool of people willing to do the work may be manually sorted. The groups will have to agree to what the criteria are and trust whomever does this to implement it correctly. Those who are responsible for performing it would have to have sufficient knowledge to securely delete unwanted files when done.

This will be impractical for most groups.

### Simple scripting

Write a simple script to decide what images to destroy and which to keep, for example, keep or destroy images

- Which were sent by certain people who have requested/agreed to it
- Attached to messages with certain keywords

It would also be possible to reduce the size of all images to, for example, 200px or less, so that you could sort of see what was the content, but so much detail would be lost that misuse would be less likely. 

### Advanced automation

I am far from qualified to write much on this, but we do know that face detection software is commonly used. Someone who knows what they are doing could use AI for sorting. Most of us do not have access to this kind of technology and the quality of results could never be guaranteed. Manually checking would probably be required. 









Personally, I would never claim to be able to make any such archive anonymous.

 

# 

 

 

 

 

 

Regarding making these messages "anonymous": The reason I was so hesitant to guarantee anything is *not* because I don't agree with the desire to have privacy, but because it is a very, very difficult (*if not impossible*) accomplish in any meaningful way and I would not want to over-promise. I am corresponding with Avery from QDHP and hopefully they will continue to take the time to communicate with me, but as it stands I am quite skeptical of this claim. I am in no way attempting to dissuade you from working with them, and I'm happy you have found someone who suits you, but I think you should have realistic expectations.

 

That said, I am truly delighted to have learned about the QDHP and hope we will be able to work cooperatively and in a way that is mutually beneficial. They have obviously been at this much longer and have many benefits vs me. In many ways they are ideal.







# Emails were never private to begin with 

Really, a mailing list is no place to put anything which one wishes to be "anonymous". 

Industries and organizations which place high value on keeping information are either reluctant or totally unwilling to use email to communicate anything sensitive. 

You may have noticed that financial institutions, medical organizations and government bodies will often send you an email to *alert you to log in to their site*, where you may retrieve a message awaiting you. However they are less likely to send you a statement, bill, medical report, tax information or similar directly through email. 

[How to Make Your Email HIPAA Compliant](https://www.paubox.com/blog/how-to-make-email-hipaa-compliant)

[HIPAA Compliance for Email](https://www.hipaajournal.com/hipaa-compliance-for-email/)







A mailing list, like Yahoo Groups, is not just an email to a single recipient, it is an email to dozens, hundreds or thousands of recipients. This multiplies the likelihood that 

 









The truth is that anyone who is a member of the Group could have done this kind of downloading process at any time without anyone ever knowing. 



In addition to being posted on the web interface and stored on yahoo's servers (probably including multiple backups and storage in different formats and different locations), each message is sent to the inboxes of all subscribers (unless they have chosen to turn such delivery off).

- Each time a message is viewed on the Yahoo site, on webmail, or in an email program (and sometimes even without being viewed), the content of it is downloaded onto their device where it may be deleted (usually in such a way that it can be easily undeleted) or kept indefinitely. *Every time you view material on the internet, it must be downloaded to your computer in some form*. This is one reason why it's so hard to stop people from keeping music and videos.
- The nature of the internet means that content does not travel directly from the mail server to the user, but rather passes trough many third parties en route. Providers of internet/data services must handle everything to get it from one place to another, and what happens to it in transit is never guaranteed to be secure.
- People use many different backup tools/services so the content has certainly been grabbed and stored under unknown conditions in those.

It is very plausible that an email (and any attachments) sent today will fairly immediately propagate itself to thousands of devices (computers, phones, servers) all around the world. A theft, break-in, hack, guessed password, confiscation by the state, human error, network glitch or any other unauthorized access to *any one of those thousands of devices* can result in the information being shared on the open internet.

 

The reason I say all this is that is not to discourage you from archiving your content, but rather to describe that it was never private in the first place. I am very aware that people operate under different assumptions and share stuff with the impression that it was somehow secret or limited access, but that was always a fiction.

 

On the question of alternatives, I have it planned to put info about that on the [site](https://archivetransyahoo.noblogs.org). Here is some rough thoughts. I'll probably clean this up a bit and use it there, no sense writing the same thing twice. I'd be obliged if you let me know of any other options you come across (with your opinions if you are so motivated) so they can be included.

 

There is a site called groups.io that the people from Internet Archive tell me lots of groups are moving to. It was apparently started by ex-yahoo people who "saw the writing on the wall" (whatever that means). They even have an import tool from yahoo groups. However they charge $$$$, and guess what, the price just doubled! What a coincidence.

 

If I was looking to create a list the first place I would look at would be https://riseup.net/en/lists Riseup.net has been around for years and years and is well regarded by lefty type folks as *probably* not agents of the state. because of the work done by their users they take privacy and security seriously.

 

In the past I have used google groups, but recently having learned about more about how *deeply creepy* google is, I have decided to stop using their products as much as possible. However it is very similar to yahoo groups.

 

 

 

 

 

 

 