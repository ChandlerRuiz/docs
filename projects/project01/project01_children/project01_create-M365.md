---
layout: page
title: Create M365 Environment
parent: On-Prem to Azure
nav_order: 2
---

# Creating the M365 Environment

Thankfully Microsoft is kind enough to lend us their resources for free utilizing the [Microsoft 365 Developer Program].

Head on over to the developer website and follow the guide below.

{: .note}
Before continuing, it's advised to use a "Private" tab in your browser so that you can properly follow along without signing into your primary Microsoft account.

---

## Joining the program and creating a Microsoft account.

Once you're on the developer page, click the ***Join now >*** button.  
![](/assets/images/projects/project01/create-M365-environment/M365-button-join-now.png "M365 - Join now")

You will be redirected to the Microsoft sign-in page.  
I will be creating an account using a new email address specifically for this lab.  
![](/assets/images/projects/project01/create-M365-environment/M365-sign-in.png "M365 - Sign in")

{: .note}
Go ahead and create an email using the `@outlook.com` domain. You will utilize this as an alternate/fallback email for your environment post-creation.  

Now choose the ***Get a new email address*** hyperlink.  
![](/assets/images/projects/project01/create-M365-environment/M365-create-account.png "M365 - Create Account")

Enter the email you'd like to create and utilize for this lab environment.  
![](/assets/images/projects/project01/create-M365-environment/M365-create-email.png "M365 - Create email")

---

## Initial Dev Environment setup.

After creating our Microsoft account, we will be redirected to the Developer Program dashboard to configure the first-time setup of our environment.

We're initially met with a screen that will walk us through some basic setup of the environment and initialize our subscriptions.  

Fill out the required sections, read the TOC and accept them if you so choose, then click ***Next***.  
![](/assets/images/projects/project01/create-M365-environment/M365-dev-join-1.png "M365 - Dev Join Page 1")

On the next screen, we will be asked how we'll be using the Developer Program. Choose whatever you like, but I have chosen ***Personal Projects*** as that is the intent for my environment.  
![](/assets/images/projects/project01/create-M365-environment/M365-dev-join-2.png "M365 - Dev Join Page 2")

You will then be asked to select your interests within the Developer Program. Do so and click ***Save***.  
![](/assets/images/projects/project01/create-M365-environment/M365-dev-join-3.png "M365 - Dev Join Page 3")

---

## M365 E5 Sandbox initialization.

After completing the initial setup of our Dev Environment, we will now activate the included M365 E5 Sandbox. You should automatically have a popup appear to complete this portion of the setup.  

{: .note}
If for some reason your dashboard doesn't auto-launch the setup process you can click the ***Set up E5 subscription >*** hyperlink to continue following along. This will be on the main page of your [M365 Developer Program dashboard].
![](/assets/images/projects/project01/create-M365-environment/M365-dev-lost.png "M365 - Dev Lost")

Moving on, we will be choosing the ***Configurable sandbox*** option so that we can use the custom domain we just purchased. Click ***Next***.
![](/assets/images/projects/project01/create-M365-environment/M365-dev-setup-1.png "M365 - Dev Setup Page 1")

Complete the next setup page as you see fit and click ***Continue***.  
![](/assets/images/projects/project01/create-M365-environment/M365-dev-setup-2.png "M365 - Dev Setup Page 2")

Complete the required security setup process with your information as required. You will get a code and need to enter it to finalize the setup. *Sorry, I missed the SC on the second screen for this one.*  
![](/assets/images/projects/project01/create-M365-environment/M365-dev-setup-3.png "M365 - Dev Setup Page 3")

Once you've verified your account setup, you will see the below screen appear.
![](/assets/images/projects/project01/create-M365-environment/M365-dev-setup-4.png "M365 - Dev Setup Page 4")

After the setup process is complete, you will be brought back to the dashboard and see that your subscription is activated. Click the ***Go to subscription*** hyperlink to navigate to your M365 Admin Dashboard.


![](/assets/images/projects/project01/create-M365-environment/M365-dev-setup-complete.png "M365 - Dev Setup Complete")

{: .note}
You will be required to sign into the M365 account you just created to access the admin dashboard.

---

## Adding your domain to the M365 Developer Program environment.

Now that we've signed up for and initialized the M365 Environment, let's add our purchased domain within the ***Domains*** section. This will allow us to fully utilize the domain across M365.  

If you've just signed into your account, or accessed the account through the ***Go to subscription*** hyperlink from the last section, you can access the admin dashboard by clicking the Admin Portal button on the sidebar.  
It looks like this -> 
![](/assets/images/projects/project01/create-M365-environment/M365-admin-icon.png "M365 - Admin Icon")<- and will be located on the sidebar to the left.

Alternatively, simply click the button below.  
[M365 Admin Portal](https://admin.microsoft.com/){: .btn .btn-blue }

Alright, now that we're at the admin dashboard, expand all the settings by clicking ![](/assets/images/projects/project01/create-M365-environment/M365-admin-siebar-showall.png "M365 - Admin Sidebar Show All")

Expand the ***Settings*** section and select ***Domains***.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-sidebar-domains.png "M365 - Admin Sidebar Domains")

At the top of the page, click ![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add.png "M365 - Domains Add Button") to initiate the wizard.

Now enter the domain you'd like to connect, then click ![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-1-1.png "M365 - Domains Add Page 1 Button") below.   
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-1.png "M365 - Domains Add Page 1")

After submitting the info for the domain we want to add, we must go through the verification process. I'm using Cloudflare so I'm able to simply sign into my Cloudflare account.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-2.png "M365 - Domains Add Page 2")

Once you've selected your verification option, click ![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-2-1.png "M365 - Domains Add Page 2 Button") to initiate the process.  

After clicking verify, I'm prompted with a login panel for Cloudflare.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-2-2.png "M365 - Domains Add Page 2 - Cloudflare")

After logging in, I was presented with a screen to *"Authorize DNS records from Microsoft"*, which will be used by Microsoft to validate ownership of the domain.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-2-3.png "M365 - Domains Add Page 2 - Authorize")

After authorizing through whatever method you've chosen, you will see the following screen while Microsoft goes through the domain validation process.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-2-4.png "M365 - Domains Add Page 2 - Verifying Phase")

After the validation process is complete, we're brought to the next step of setup.  

We need to connect our validated domain to our M365 Environment.  
Again, since I'm using Cloudflare, I can use the built-in process to append the required records. Once you've made your selection for how you'd like to connect your domain, click ![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-3-1.png "M365 - Domains Add Page 3 - Continue") to proceed.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-3.png "M365 - Domains Add Page 3")

Microsoft now wants us to verify whether or not it should be adding the required DNS records for Exchange services.  
  
For this project, we will not be utilizing any on-premise Exchange Servers, so we can accept the defaults and click ![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-3-3.png "M365 - Domains Add Page 3 - Add DNS Records") to continue.  

Microsoft is once again asking for authorization to append DNS records on our behalf for functionality between the domain and M365 services. Select ![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-3-5.png "M365 - Domains Add Page 3 - Authorize Button") to continue.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-3-4.png "M365 - Domains Add Page 3 - Authorize")

After authorization is confirmed, we're met with another loading screen.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-3-6.png "M365 - Domains Add Page 3 - Checking DNS Records")

After some time, we're brought back to the overview of adding our domain, where we should receive a message stating *"Domain setup is complete"*. Click ![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-4-1.png "M365 - Domains Add Page 4 - Done") to exit the setup.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-add-4.png "M365 - Domains Add Page 4 - Complete")

---

## Congratulations!  
We've successfully added a domain to our M365 Environment and can see it in the ***Domains*** section.  
![](/assets/images/projects/project01/create-M365-environment/M365-admin-domains-overview.png "M365 - Domains Overview")


[Microsoft 365 Developer Program]: https://developer.microsoft.com/en-us/microsoft-365/dev-program
[M365 Developer Program dashboard]: https://developer.microsoft.com/en-us/microsoft-365/profile