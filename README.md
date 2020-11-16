# [Eventarc](https://www.google.com) FAQ

⚠️ Beware: This is a community-maintained informal knowledge base.

It does not reflect Google’s product roadmap. (Please don't ask when a feature will ship)
Refer to the Cloud Run documentation for the most up-to-date information.
Googlers: If you find this repo useful, you should recognize the work internally, as I actively fight for alternative forms of content like this.

Is this repo useful? Please ⭑Star this repository and share the love.
Curious about something? Open an issue, someone may be able to add it to the FAQ.
Contribute if you learned something interesting about Cloud Run.
Trouble using Cloud Run? Ask a question on Stack Overflow.
Check out awesome-cloudrun for a curated list of Cloud Run articles, tools and examples.
Follow me on Twitter as I frequently share Cloud Run news and tips.

* Test1
* Test2

* Basics
 * [Q1]()
 * [Q2]()

## Q1

## Q2

Are Cloud Run's Eventarc and Cloud Functions Events and Triggers  basically the same thing under the hood? Seems like both do Pub/Sub, but CF has some nice wrapping for Storage/Firebase/Firestore.

I'm curious about a few things:
1) Is one or the other the future, or will both continue to evolve?
2) Will Eventarc always be Cloud Audit-over-Pub/Sub or will it get direct paths for things like Firestore?
3) Are there differences in latency, availability, throughput between the two paths?
--
Hello,

An approximate timeline for Eventarc to be available in asia-northeast1 region is Q2/Q3 of 2021.

We'd love to learn more about the specific customer and their use case, do you have any information you can share?

Regards
Prashant

On Thu, Nov 12, 2020 at 12:28 AM Utchy / Kazuki Uchima <kuchima@google.com> wrote:
Hi Prashant,

I'm Utchy, Application Modernization Specialist in Japan.
IHAC who is interested in Eventarc, they asked me that when the Eventarc will be available in Tokyo (asia-northeast1) region.
Do we have any timeline for the Tokyo region release?

Thank you for your support.

Regards,
Utchy

--
Hey Prashant,
Thanks for adding us to the list. We are about to start on the events and have few things to get clarified before having our hands dirty.

1. We see Cloud run events supporting 60+ services through audit log events. We mainly want to use Firestore triggers functionality on cloud run so that we can totally move out of cloud functions. 

We would like to know how reliable are audit log events? We want to use the events for invalidating Redis cache. So would like to know if there are any limitations in choosing Audit log events.

2. Are firestore trigger events scheduled for cloud run?
