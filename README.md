# How to generate a Key
🚀 Upload Folder to GitHub Using SSH (Simple Guide)
✅ 1. Create SSH key (if not already done):

ssh-keygen -t ed25519 -C "your_email@example.com"

    press enter through the prompts

✅ 2. Add SSH key to GitHub:

cat ~/.ssh/id_ed25519.pub

    copy the output

    go to github.com/settings/keys

    click “New SSH key”, paste, save

✅ 3. Test SSH connection:

ssh -T git@github.com

    should say:
    “Hi your-username! You’ve successfully authenticated…”

✅ 4. Create your GitHub repo (on the website)

    don’t add a README/license

    get the SSH URL, like:
    git@github.com:your-username/your-repo.git

✅ 5. In your project folder:

git init
git remote add origin git@github.com:your-username/your-repo.git
git add .
git commit -m "Initial upload"
git branch -M main
git push -u origin main

and that’s it! your folder will be live on GitHub via SSH 🎉

want me to turn that into a reusable .sh script version?" can convert you in read.md format so i copy pls
