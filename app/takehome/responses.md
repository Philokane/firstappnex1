### 1. From this list, rank your 5 most favourite and 5 least favourite support tasks. Provide a brief explanation for each.**

### Most favourite tasks

1. **Write and maintain support articles and docs pages**

    It is vital that good internal and external documentation is maintained. This should be easy to read and understand, up-to-date and answer the questions an end-user may have, while also sign-posting to where other information can be found for deeper knowlefge or further assistance.

2. **Scheduling time-off coverage and collaborating as part of a growing cohesive support team**

    Working as part of a team is a vital part of ensuring that the business runs smoothly - managing time-off coverage ensures that the team is

3. **Manage a support team**

    For me managing a support team is about understanding the goals and aims of the business and how the team can better meet these goals. I use my knowledge as a support team member as well as the technical tasks performed by the support team to understand the goals of the team, as well as the skills of each team-member, and how this can be utilised to improve the running of the business.

4. **Help train and onboard new support teammates**

    Sharing my knowledge to new team-members is an important part of my role. I maintain strong personal documentation that I am able to share among team-members and I ensure those around me have the information they need to be great at their job.

5. **Respond to queries on Twitter, Reddit, Hacker News and other 3rd party sites**

    It is important that the company keeps in touch with the developer community and is able to see where the users are in order to fully understand the user-base as well as improving the services and products offered. I am comfortable communicating in these spaces as I see the importance of being in the spaces that our users and customers are.

### Least Favourite tasks

1. **Find and recruit teammates for the support team**

    I am more comfortable working with current team-members and don’t have the skills required in finding and recruiting new members.

2. **Work with 3rd party partners to track down a tricky situation for a joint customer**

    While this will take a lot of work, I am more comfortable working through a number of issues in order to assist a number of users and customers over spending a long time on a single issue.

3. **Dig through logs to troubleshoot a customer's broken project**

    When I get bogged down on an issue that I’m stuck on, I will often spend more time than necessary, which can lead to other work or projects being neglected. In order to ensure this does not happen I will set timers and block time on my calendar. However, due to the requirement to be fully aware of time while working such a task, I will mark this as something that would not be a preference.

4. **Create video tutorials to help teach users a specific feature or use case**

    I’m not comfortable recording myself on video, however I am always happy to demonstrate how a task is performed or how to use a specific feature in-person or on a Zoom call.

5. **Help resolve billing issues for customers**

    I’m comfortable working technical issues rather than billing concerns. Whenever these issues arise, I will do what I can in order to understand the customer’s use-case offer a good solution, however I will revert to the billing team for bill-specific issues,

### 2. What do you want to learn or do more of at work?

There are many areas that I want to develop my skills, this ranges from networking, to research to code-development. Currently, the main area I hope to improve is my time management skills. This is a continual work in progress and something I am always developing. Time management leads to improved decision making, increased productivity, higher quality of work, and improved work-life balance; these are all areas that I continue to work on and never want to neglect.

**Coding**
I'm very technically minded, but I'm only okay with code. I can work with other people's code, but I'm not so hot with writing my own. Were I to find a home at Vercel, I'd really love the opportunity to take advantage of the resources and people in a company like this, and finally learn to code in earnest. I have experience with a number of languages, however I want to develop stronger knowledge of more advanced code skills.

**Cloud Infrastructure knowledge**
My cloud knowledge is good - but I want to continue to develop this in order to understand exactly the methods of building out large applications using a number of distributed services with failover and fallback plans in place.

### 3. Describe how you solved a challenge or technical issue that you faced in a previous role (preferably in a previous support role). How did you determine that your solution was successful?

When troubleshooting issues I use the following troubleshooting methodology:

- Identify the problem
- Establish a theory of probable cause
- Test the theory to determine the cause
- Establish a plan of action to resolve the problem and identify potential effects
- Implement the solution or escalate as necessary
- Verify full system functionality and, if applicable, implement preventive measures
- Document findings, actions, outcomes and lessons learned

One recent occasion where I used this was in my role at Fastly was in determining why the correct TLS Certificate was not serving on the customer’s website as expected.

On this occasion, the problem was identified using openssl tool to identify the certificate being served. Using command line tools I investigated where the site was being hosted and where the DNS was pointing. This helped identify that the correct DNS anycast records were not being used on the domain that would point the domain to the correct backend on the Fastly network that hosted the updated certificate.

Once the solution had been identified, the customer was told how to make the change with their DNS provider and the correct DNS records were provided.

Specific steps were written in detail to the customer in an email ticket which allowed them to make the changes required.

Once confirmed that the changes were made I confirmed this on my end and waited until the DNS had propagated. Once the domain was being served by the correct DNS records, the updated TLS certificate displayed and the error cleared. These findings were documented to the customer with links to the documentation provided for next time the change is required.

### 4. When would you choose to use Edge Functions, Serverless Functions, or Edge Middleware with Vercel?**

**Edge Functions**

Use for lightweight functions that need to execute close to the end-user across a global network. Caching is available when using edge functions. Best for real-time data streaming and authentication processes.

**Serverless Functions**

Serverless functions are ideal for building websites and web apps, allowing developers to focus on the core product without having to set up or maintain infrastructure. Serverless Functions, usually execute in one specified **region** (although this can be configured), and allow you to write small chunks of code to provide additional functionality in your application, such as handle authentication, stream data, and make database queries. This is used if running Node.js.

**Edge Functions**

Edge Functions are used for for low-latency global execution. Responses from Edge Functions can be *cached* and *streamed* in real time. Globally distributed by default. Lightweight with a slim runtime. Pricing is based on compute time.

### 5. Imagine a customer writes in requesting help with a build issue on a framework or technology that you've not seen before. How would you begin troubleshooting this and what questions would you ask the customer to understand the situation better?

If the customer is asking about a framework or technology I have not seen before I will first research the area. I will start by looking at the Vercel documentation, both internal and external. If this does not yield helpful results I will search Google, pin-pointing results from Stack Overflow and [Dev.to](http://Dev.to) as places known for strong updates on the latest technologies.

In order to troubleshoot the issue, I would ask the customer what they are hoping to achieve, the steps they have taken and errors they’re receiving. I will ask for screenshots and response outputs.

Once I have a full understanding of what they hope to achieve I will do my best to provide sufficient information to them. If I still require further guidance I will speak with someone in my team who has knowledge in this area followed by asking in an appropriate channel before escalating the ticket internally.

### 6. The customer from question 5 replies to your response with the below: “I’m so frustrated. I’ve been trying to make this work for hours and I just can’t figure it out. It must be a platform issue so just fix it for me instead of asking me questions.” Please write a follow-up reply to the customer.**

Hi [name]

I understand that this can be frustrating, however I hope to work with you in order to get the best method of resolving your issue. As we don’t have specific documentation on this technology which is limiting the answers and speed at which I can assist you. I hope you will accept my apologies for the time it has taken to resolve your issue.

In order to get your moving, we require as much detail as possible on the particular technology you’re using, your use-case and what you are hoping to achieve.

I will be escalating your ticket to our more senior team, where a senior engineer with experience in this technology will provide you with further guidance.

### 7. A customer writes in to the Helpdesk asking "How do I do a redirect from the /blog path to [https://example.com](https://example.com/)?" Please write a reply to the customer. Feel free to add any information about your decision making process after the reply

There are a number of ways to implement a redirect within Vercel.

To redirect from `/blog` path to [`https://example.com`](https://example.com/) on Vercel, you can add the following redirect rule in your vercel.json file:

```jsx
{
  "redirects": [
    {
      "source": "/blog/:path*",
      "destination": "/news/:path*"
    }
  ]
}
```

Here's how this redirect rule works:

- **`"source": "/blog/:path*"`** matches any incoming request that starts with **`/blog/`**, capturing the remaining path in the **`:path*`** wildcard parameter.
- **`"destination": "https://example.com/:path*"`** constructs the redirect URL by appending the captured **`:path*`** to **`https://example.com/`**.
- **`"permanent": true`** specifies that this should be a permanent 308 redirect, which is cached by clients and beneficial for SEO
- `**statusCode`** An optional integer to define the status code of the redirect. Used when you need a value other than 307/308 from `permanent`, and therefore cannot be used with `permanent` boolean.

For more detail on this please see the below documentation pages:

- <https://vercel.com/docs/edge-network/redirects#adding-redirects>
- <https://vercel.com/docs/projects/project-configuration#redirects>
- <https://vercel.com/docs/edge-network/redirects#adding-redirects>

### 8. A customer is creating a site and would like their project not to be indexed by search engines. Please write a reply to the customer. Feel free to add any information about your decision making process after the reply

Hi [name]

This is Phil in the Support Team, thanks for reaching out with your query.

In order to prevent search engines from indexing your Vercel site the `X-Robots-Tag` header will be used. Vercel [Preview Deployments](https://vercel.com/docs/platform/deployments#preview) are **not indexed by search engines** by default because the **`X-Robots-Tag`** HTTP header is set to `noindex`.

If you are using a [Custom Domain](https://vercel.com/docs/custom-domains) that is assigned to a non-[Production Branch](https://vercel.com/docs/git#production-branch), however, the header `X-Robots-Tag: noindex` **will not** be set.

To confirm the value of the `X-Robots-Tag` header, you can use the following [curl](https://curl.haxx.se/) (already available on most desktop devices) command in your terminal to check your Preview Deployment's headers:

```jsx
curl -I <preview-deployment-url>
```

The response will look like this:

```jsx
x-robots-tag: noindex
```

For detail on adding the appropriate response header to your code on a custom domain please see the documentation page here: <https://vercel.com/guides/are-vercel-preview-deployment-indexed-by-search-engines>

If you have any other issues or specific questions regarding HTTP headers please let me know.

In this response, I have added some detail that will answer the customer’s question quickly, while providing the documentation page and directions to enable the full response which can be found on the documentation.

### 9. What do you think is one of the most common problems which customers ask Vercel for help with? How would you help customers to overcome common problems, short-term and long-term?

My understanding is that build issues would be the most common - this includes understanding build errors and logs.

I would help customers overcome these issues in short-term by ensuring public documentation is kept up-to-date and easily searchable for questions and answers.

A long-term solution may be an ‘academy’ or educational programme that users can complete in order to become familiar with the platform and understand it fully.

### 10. How could we improve or alter this familiarisation exercise?

- Some of the tasks are repetitive. With a number of options available and not a lot of detail provided in the questions.
- It is difficult to gauge the response required.
