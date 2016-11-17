## Customize Your Cygwin

**STEP 1**  

Launch Cygwin and enter `ls -a` to see your **.bash_profile**

**STEP 2**

From Cygwin, enter `atom .bash_profile` or `atom.cmd .bash_profile` to open your **.bash_profile** in Atom.

**STEP 3**  

Add the following Bash script to your **.bash_profile**.

```bash
alias ls="ls --color=auto"
LS_COLORS="di=34;1:ln=36;1:ex=31;1:fi=30:*~=31;1:*.html=31;1:*.shtml=37;1"
export LS_COLORS
```
To help understand what's happening in this Bash script, see this [askubuntu post](http://askubuntu.com/questions/466198/how-do-i-change-the-color-for-directories-with-ls-in-the-console).

**STEP 4**

Save your **.bash_profile**, head back over to Cygwin, and run:

```bash
source .bash_profile
```
Next, enter `ls` to confirm that your output now contains colors.

**STEP 5**

If you'd like to change your Cygwin background color and text color, right-click over the Cygwin window and choose **Options** or **Properties**. To change the background, select **Looks** > **Background**, then adjust your background color and select "Okay." For text color, select **foreground**, choose a new color, then select "Okay." 
