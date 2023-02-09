# Website Deployment & Custom Domain - Week 4

### Greetings! 👋

For this week, I'll be documenting the process of deploying a project to Netlify, then configure a custom domain and connect it to Netlify through Cloudflare.

## Link to Website

### [https://archstudiosite.xyz/](https://archstudiosite.xyz/)

![markdown-website](/assets/markdown/markdown_image.png)

---

## 🛠️ Deployment Setup

### 1. Sign Up / Log In to Netlify

![netlify-1](/assets/markdown/netlify-1.png)

After signing in, you should be greeted with the following page.

![netlify-2](/assets/markdown/netlify-2.png)

### 2. Project Setup

- Import project by navigating to **Sites** and click **Add new site > Import an existing project**.

![netlify-3](/assets/markdown/netlify-3.png)

- Select one of the Git provider.

![netlify-4](/assets/markdown/netlify-4.png)

- Select a repository to connect.

![netlify-5](/assets/markdown/netlify-5.png)

- Leave the settings at default and click **Deploy site**.

![netlify-6](/assets/markdown/netlify-6.png)

- Congrats! Your page should look like as shown below and the site can be accessed by clicking the higlighted link next to your site preview.

![netlify-7](/assets/markdown/netlify-7.png)

## 🌐 Custom Domain Setup

To use a custom domain, you need to purchase a domain name through a Domain Name Registrar.

For this case, I will be using Niagahoster.

![domain-1](/assets/markdown/domain-1.png)

### 1. Buy a domain

- Type your prefered domain name on the search bar. A suggestion will be shown if its available (or scroll down for more domain alternatives).
- Click **Pilih** on your prefered name to continue check-out page.

![domain-2](/assets/markdown/domain-2.png)

- Select your usage duration for the domain name, then click **Lanjutkan**.
- You will be redirected to select payment method and complete the transaction.


![domain-3](/assets/markdown/domain-3.png)

- After completing your payment, you should be greeted with a page as shown below. Congrats! You have successfuly purchased your domain name!

![domain-4](/assets/markdown/domain-4.png)

### 2. Clouflare Setup

- If you don't have an account, sign up on Cloudflare's website then log in to access the **Dashboard**, which should look like this.

![domain-5](/assets/markdown/domain-5.png)

- On the top navigation bar, click **Add site**, then type your purchased domain name and click the **Add site** button.
- You will be redirected to select a Cloudflare Plan. Select the **Free** Plan and click **Continue**.

![domain-6](/assets/markdown/domain-6.png)

### 3. Change Nameservers 

- Follow the instructions given by Cloudflare to replace the two nameservers currently in use on Niagahoster.

![domain-7](/assets/markdown/domain-7.png)

- On the previous Niagahoster page, under **Overview Domain**, click the **Ubah Nameserver** button. Replace Nameserver 1 & 2 with nameserver from Cloudflare as shown below, then click **Simpan**.

![domain-8](/assets/markdown/domain-8.png)

- Go back to the Cloudflare Dashboard and wait for it to process the nameservers. Cloudflare is active when the Overview page are shown as below.

![domain-9](/assets/markdown/domain-9.png)

### 3. Custom Domain Setup

- On the sidepanel, Go to the **DNS > Records** page and click **Add record**.
- Add the CNAME with your Netlify link as shown below, then click **Save**.

![domain-10](/assets/markdown/domain-10.png)

- Go to your Netlify project page and click **Set up a custom domain**.

![domain-11](/assets/markdown/domain-11.png)

- Type your purchased domain name.

![domain-12](/assets/markdown/domain-12.png)

- It will take a while before you can access the site. Refresh the page to check if the site is active as shown below. Congrats! You have finished setting up your custom domain!

![domain-13](/assets/markdown/domain-13.png)
