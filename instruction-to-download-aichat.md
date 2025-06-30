**Hey Kalvians!**

<p align="center">
  <img src="https://media.tenor.com/Klzqm1DesDgAAAAi/hi-emo.gif" width="150" />
</p>

You’re about to install and launch your very own **local AI environment** using **`aichat`** — a powerful, all-in-one AI command-line tool. With it, you’ll be able to run **Gemini models**, explore the **LLM Playground**, and even compare models side by side using **LLM Arena**.

By the end of this lesson, your **local AI workspace** will be ready for all upcoming sessions. Let’s go!

---

## What You Will Do

* Install `aichat` for your OS (Windows / Linux / macOS)
* Configure it with your **Gemini API Key**
* Add `aichat` to your **system path** to run it from anywhere
* Launch your **local AI server**
* Access the **LLM Playground** and **LLM Arena** from the browser
* Chat, test, and compare LLM responses side-by-side

---

## What is aichat?

`aichat` is your personal AI terminal tool. It allows you to:

* Chat with **LLMs like Gemini** directly from your terminal
* Use a full web interface via **LLM Playground** and **LLM Arena**
* Compare different models easily
* Run your AI environment **locally with your own key**

> Think of it like having your own ChatGPT — but on your own machine and fully customizable.

---

## Installation Guide (Select Your OS)

Choose your operating system below and follow the steps carefully.

---

## For Windows Users

<div align="center">
  <iframe src="https://drive.google.com/file/d/1s3TUjVslJbA15SO6oN-ZTQ-ttni5HNyG/preview" width="650" height="400" allow="autoplay"></iframe>
  <p><em>aichat Installation Video</em></p>
</div>

## Steps

1. Visit: [https://github.com/sigoden/aichat](https://github.com/sigoden/aichat)

2. Download the latest ZIP for Windows under **Releases**

3. Extract the ZIP file to a folder (e.g., `C:\aichat`)

4. Double-click on `aichat.exe`

   You’ll see:

   ```
   ? No config file, create a new one? (Y/n)
   ```

5. Type `Y` and hit Enter

6. Use arrow keys to choose **`gemini`** as your API provider → hit **Enter**
7. When prompted for your **API key**, go to [Google AI Studio](https://aistudio.google.com/), get your key, and paste it into the terminal
8. Next, you will see a model selection prompt like this:

```
? Default Model (required):
> gemini-2.0-flash
  gemini-2.0-flash-lite
  gemini-2.0-flash-thinking-exp
  gemini-2.0-pro-exp
  gemini-2.5-pro-exp-03-25
  gemma-3-27b-it
  gemini-1.5-pro-latest
[↑↓ to move, enter to select, type to filter] 
```

* Use your **Up (↑)** and **Down (↓)** arrow keys on your keyboard to scroll through the list of available models.
* Select **gemini-2.0-flash** and press **Enter**.

9. After selecting your model, the program will confirm with:

```
Welcome to aichat 0.29.0
Type "help" for additional help.
```

10. Now try typing a greeting, for example:

```
Hi, I am YOUR_NAME
```

You should get a response from the AI!


---

##  Add to Windows PATH

1. Press Windows Key → search **Environment Variables**
2. Click **Edit the system environment variables**
3. In the dialog → click **Environment Variables**
4. Under **System Variables**, select `Path` → click **Edit**
5. Click **New** and paste your folder path (e.g., `C:\aichat`)
6. Click OK → OK → OK

Now, open a new terminal and run:

```
aichat --version
```

It should show the version — now you're all set to use it anywhere!

---

## For Linux Users

## Steps

1. Go to [https://github.com/sigoden/aichat](https://github.com/sigoden/aichat)

2. Download the `.tar.gz` file for Linux

3. Extract using:

   ```bash
   tar -xvzf aichat-<version>.tar.gz
   cd aichat-<version>
   ./aichat
   ```

4. On first run, you’ll see:

   ```
   ? No config file, create a new one? (Y/n)
   ```

5. Type `Y` and hit Enter to create a new config
6. Use arrow keys to move the highlight to **`gemini`** → press **Enter**
7. When asked for your **API key**, get it from [Google AI Studio](https://aistudio.google.com/) and paste it into the terminal.
8. You will then see a model selection menu like this:

```
? Default Model (required):
> gemini-2.0-flash
  gemini-2.0-flash-lite
  gemini-2.0-flash-thinking-exp
  gemini-2.0-pro-exp
  gemini-2.5-pro-exp-03-25
  gemma-3-27b-it
  gemini-1.5-pro-latest
[↑↓ to move, enter to select, type to filter] 
```

* Use the **Up (↑)** and **Down (↓)** arrow keys to highlight the model you want.
* Select **gemini-2.0-flash** and press **Enter**.

9. After selecting the model, you will enter the chat mode.

---

## Add to Linux PATH

To make `aichat` available globally:

1. Find your extracted folder path, e.g.:

   ```
   /home/youruser/aichat-folder
   ```

2. Edit your profile file (depending on your shell):

   ```bash
   nano ~/.bashrc
   # or for zsh
   nano ~/.zshrc
   ```

3. Add this:

   ```bash
   export PATH="/home/youruser/aichat-folder:$PATH"
   ```

4. Save → exit → reload:

   ```bash
   source ~/.bashrc
   # or
   source ~/.zshrc
   ```

5. Try:

   ```bash
   aichat --version
   ```

---

## For macOS Users

## Steps

1. Go to [https://github.com/sigoden/aichat](https://github.com/sigoden/aichat)

2. Download the `.tar.gz` file for macOS

3. Extract using:

   ```bash
   tar -xvzf aichat-<version>.tar.gz
   cd aichat-<version>
   ./aichat
   ```

4. On launch:

   ```
   ? No config file, create a new one? (Y/n)
   ```

5. Type `Y` and press Enter to create a new config
6. Use arrow keys to select **`gemini`** → press Enter
7. Paste your Gemini API key copied from [Google AI Studio](https://aistudio.google.com/)
8. Next, you’ll see the model picker prompt:

```
? Default Model (required):
> gemini-2.0-flash
  gemini-2.0-flash-lite
  gemini-2.0-flash-thinking-exp
  gemini-2.0-pro-exp
  gemini-2.5-pro-exp-03-25
  gemma-3-27b-it
  gemini-1.5-pro-latest
[↑↓ to move, enter to select, type to filter] 
```

* Navigate the list using **Up (↑)** and **Down (↓)** arrow keys.
* Select **gemini-2.0-flash** and press **Enter**.

9. Once the model is selected, you’re ready to start chatting!


---

## Add to macOS PATH

1. Find the folder path, e.g.:

   ```
   /Users/yourname/aichat-folder
   ```

2. Open your profile:

   ```bash
   nano ~/.zshrc
   # or for older versions
   nano ~/.bash_profile
   ```

3. Add:

   ```bash
   export PATH="/Users/yourname/aichat-folder:$PATH"
   ```

4. Save → exit → reload:

   ```bash
   source ~/.zshrc
   ```

5. Try:

   ```bash
   aichat --version
   ```

---

## Run the Local AI Server

Now let’s get your local server live!

Open a terminal, then run the following command:

```bash
aichat --serve
```

You’ll see output like:

```
Chat Completions API: http://127.0.0.1:8000/v1/chat/completions
LLM Playground:       http://127.0.0.1:8000/playground
LLM Arena:            http://127.0.0.1:8000/arena?num=2
```

Open these in your browser to explore.

---

## Try the LLM Playground

* Go to: [http://127.0.0.1:8000/playground](http://127.0.0.1:8000/playground)

<p align="center"><img src="https://kq-storage.s3.ap-south-1.amazonaws.com/Simulated+Work/aichat-playground.png" width="1000"/></p>
* Type prompts like: `Tell me a fun fact about space!`

---

## Explore the LLM Arena

* Go to: [http://127.0.0.1:8000/arena?num=2](http://127.0.0.1:8000/arena?num=2)

<p align="center"><img src="https://raw.githubusercontent.com/sahil-kalvium/Images/main/aichat-arena.png" width="1000"/></p>
* Select different models and compare their responses
* Great for testing reasoning, creativity, and output formats

---

## Final Checklist

* Installed `aichat`
* Configured Gemini key via terminal and selected `gemini-2.0-flash` as the default model
* Added to `PATH` for easy usage
* Tested on terminal and browser
* Ran `aichat --serve` successfully

---

## Pro Tips

* Double check your Gemini API Key — no spaces or errors!
* Always use **new terminal windows** after editing PATH
* Use the Playground and Arena links only when `aichat --serve` is running

---

<p align="center">
  <img src="https://media.tenor.com/8GcYClbSpNQAAAAi/wabisabip-wabi.gif" width="200" />
</p>

<p align="center"><em>Your AI journey is now real — and it lives on your machine!</em></p>

