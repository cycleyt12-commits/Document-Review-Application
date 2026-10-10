# Document-Review-Application
Hello guys. This is my document review app where I am going to be building an app in Python (with the help of other tools like codex, different AI LLM's, React, Azure) which is gonna basically review and read any document and help the user with the decision. For more information , make sure to read the README.md. . Inspired by Dave Ebbelaar.

ABOUT ME:  My name is Peter. I am a 14 year old soon-to-be entrepreneur learning the necessary skills for my business. I want my future business to be an AI Agent, system or SaaS builder for other companies, solo business only by me (B2B). Looking forward to having my own AI big Company when I am older and wish for the best.  If you wish to help me in my journey and have a partnership, contact me on shapetru1108@gmail.com.

ABOUT THE APP : MUST KNOW : This isn't an app that I am planning to sell, maybe for my personal use. Just trying to get more experience about what it's like to build apps and the whole process. 
What I will build : 
    A hybrid extraction pipeline on Azure, with Document Intelligence as the primary extractor and Azure OpenAI in a supporting role
    Deterministic finance rules in plain Python, because models extract evidence but code decides policy
    A FastAPI backend with SQLite persistence and a React review portal built around the reviewer's workflow

The project is also a course in Azure itself. You create an account with free credits, work with the Azure CLI instead of clicking through the portal, and learn what resource groups, tiers, and regions actually mean when you provision real services.
The build must do: 
    Accept one PDF or image per upload, with a 4 MB limit
    Recognize whether the document is an invoice or a receipt automatically
    Extract supplier and customer details, VAT IDs, dates, purchase order, currency, totals, and line items
    Validate EU VAT number formats offline and reconcile subtotal, VAT, and total
    Apply separate deterministic policies for invoices and receipts, including duplicate detection
    Suggest a GL account from a fixed Northstar catalog, with the reviewer able to override
    Let user correct fields, approve, reject, and draft (never send) a supplier correction email
    Keep a review history with explicit deletion so a demo can be reset

Just as important is what stays out. No authentication, no queues, no email ingestion, no accounting-system integration. This is a teaching skeleton that keeps the engineering boundaries visible, not a production accounts-payable product.

You should be able to describe, without mentioning any implementation.

User story (not real, for specific purposes only) : 

    As a finance administrator at a European company, I want to upload a multilingual invoice or receipt and receive a prepared review containing the best combined extraction, VAT and policy results, and a suggested GL account so I can approve valid documents quickly and turn supplier errors into a clear correction request.

Basically, my made user does not want an autonomous system that approves invoices. he wants a prepared review. The app does the reading, checking, and suggesting; he keeps the decision. That distinction drives everything that follows.

