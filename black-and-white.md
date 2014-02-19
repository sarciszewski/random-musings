```
This was the article I submitted to 2600: The Hacker Quarterly
I hereby release it into the Public Domain
```
About two years ago, I was a computer engineering undergraduate at UCF, hoping to eventually go to graduate school and eventually earn a Ph.D. One day, my curiosity got the best of me. I went to infragardtampabay.org and decided, "This website is used by the FBI, another Infragard site just got hacked by LulzSec. I'm no skilled hacker, so if I just looked around it should be harmless enough. I probably won't find anything." How many 2600 readers told themselves that before?

Before trying anything too obvious and noisy (SQLi), I decided to view the page source and see what software they used. This is what I saw on June 21, 2011:
```html
<!-- DotNetNuke - http://www.dotnetnuke.com                                          -->
<!-- Copyright (c) 2002-2008                                                          -->
<!-- by DotNetNuke Corporation                                                        -->
```
"Strange," I thought, "2011 is half-gone. Why would a website used by federal law enforcement show 2008 in their credits?" So I did the obvious thing: I typed "DotNetNuke vulnerability" into Google and found this page: http://www.exploit-db.com/exploits/12700/

The total "intrusion" lasted only 23 minutes, according to court documents.

Stricken with horror and disbelief of having found a published vulnerability in a website used by federal law enforcement (and having been unable to locate their webmasters' email address), I decided to blow the whistle on Twitter, various forums, and my personal website. Many experienced 2600 readers will realize this as a classic "completely stupid move" (runner up: Not using Tor, an overseas VPN, or an SSH tunnel when I knew how). I agree.

One month later, at the height of the LulzSec media frenzy, the FBI raided my dorm room and questioned me on every detail of the incident. I was then arrested, thus making me miss my scheduled exam in Discrete Structures. When I was released that evening, my face was all over the news.

I had juxtaposed my face over the "Lame Pun Coon" background, as an inside joke with my friends, and added the flavor text "How dare you accuse me... of PUNditry?!" and many media outlets chose to crop it to "How dare you accuse me", apparently for comic relief. My home town, however, opted to take the yellow brick road:
http://www.winknews.com/Local-Florida/2011-07-20/What-is-North-Fort-Myers-alleged-hacker-accused-of-doing

(A full day after, they somehow thought I had a botnet and DDoSed Infragard to get in. Despite being criticized by many people, they never corrected their mistake.)

Before anything got resolved by the courts, UCF held a student conduct hearing. When a hearing happens, you have two choices: An administrative hearing, where one adult UCF employee hears your case and decides your fate, or a peer hearing, where two UCF employees and two students decide your fate. I chose the latter, thinking that the student body would realize how benign (although admittedly reckless and stupid) my actions were in the grand scheme of things.

One of the employees was a narcissist who told the receptionist he was there for "the administrative hearing" and was evidently butthurt that he didn't have all the power throughout the hearing. The two students were meek and ineffectual. My public defender was not notified and was in fact not allowed to be present. As usual, the game was rigged, and I lost: Two year suspension (on top of whatever sanctions the court decided), and to write a 5 page apology paper.

The final decision to suspend me through Fall 2013 came right after my final exam grades were posted (I got a C in computer science 1, and a D in Physics 3; not great but I was dealing with a lot). That didn't matter to UCF though: My last semester was erased (which screwed up my taxes for the next year and is probably illegal).

Eventually, my public defender advised me that the best option would be to plead guilty to avoid prison. On an initial filing from Infragard's hosting and cybersecurity company (which I found out about in the Pre-Sentence Report), Sylint Corporation (usinfosec.com) claimed damages from June 16-24, totalling over $32,000 in damages (which meant: prison and an overwhelming restitution). When I pointed out that I don't own a time machine and couldn't have hacked them at any time before June 21, they amended their claim: $9370 in damages (45 man-hours) from the 21st through the 27th.

All this, for being a greenhorn with no knowledge of the laws or ethics surrounding computers. For being a curious and stupid kid. For the digital equivalent of knocking on someone's front door, it swinging ajar, looking in, seeing nobody home, going on my way, and then being put on house arrest for six months (and probation for five years) and told to pay the homeowner $9,370 plus $100 in Special Assessment fees. For the equivalent of a full disclosure without notifying the vendor ahead of time. I'm still amazed that they can operate while paying their employees over $200 an hour. Nepotism pays, I guess.

That was my story; since I began reading 2600, I've heard similar elements from many other people less fortunate than myself (my heart goes out to anyone locked up in prison for out-mathing or out-logicing the developers who produced a "protected system").

There is a lesson to be learned from all this, and this is what I would like to emphasize: DO NOT BE A GOOD GUY. It never pays off.

Let's look at another example: The same year I was arrested, I read news stories about a young man in the UK who hacked Facebook, and was arrested while writing his vulnerability assessment report for their whitehat challenge (https://facebook.com/whitehat). He had previously been rewarded for finding flaws in Yahoo and other large companies' websites (and was publicly acknowledged for doing so), and when the authorities interrogated him he referred them to a Cambridge lecture on Computer Science. Ring any bells? I can't find the story anymore.

I won't even get into Weev's story, because everyone knows it and this article is long enough. (Look up "weev ipad" in Google if you're curious.)

Are you seeing the pattern? Well-meaning folk are being prosecuted left and right, while the people who are causing the real damage are either on their payroll (usually as informants) or scot-free. And we wonder why our country's cyber-readiness is ranked 3 out of 10 by the NSA. In the words of Mercedes Haefer, in response to Keith Alexander's comment about how hackers are just what this country needs: "THEN STOP ARRESTING US!"

That won't happen. Government employees are overworked or lazy (depending on your perspective) and will always opt for the lowest hanging fruit. That's why HackForums blocks Tor exit nodes and known proxies. (And can you even count the number of Groups and Crews who conduct their membership interviews over Skype without causing an integer overflow? Probably not :P)

The time for the whitehat is over. Unless you have a solid contract and previous working relationship, helping a company or government agency is just opening the door to being used and abused. A whitehat is like a condom: You're either useful or disposable.

If your good nature won't let you abandon the whitehat path, let me make a friendly recommendation: don't help companies, don't help schools, don't help the government. Only help people; and even then, only do so safely and anonymously. Being anonymous should be your first priority. You can't trust anyone. TOR and proper OpSec (see also: grugq.github.io) are your essentials.

The law is black and white. You're either a criminal or not. (Most likely: you are.) While most of the hackers I've met are varying shades of gray, I think everyone could do well by taking a phrase out of the FBI's dictionary, and "go dark."
