# 💎 The Ultimate Git Reference — راهنمای جامع و نهایی گیت

This is the complete Git guide including all essential, advanced, and professional commands.
این یک راهنمای کامل شامل تمام دستورات ضروری، پیشرفته و تخصصی گیت است.

---

# 🧩 1) Setup & Configuration — تنظیمات اولیه

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git config --global user.name "..."` | تنظیم نام کاربری | Sets your username. |
| `git config --global user.email "..."` | تنظیم ایمیل | Sets your email. |
| `git config --list` | نمایش تنظیمات | Shows the current configuration. |

---

# 🌱 2) Repository — ساخت و دریافت مخزن

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git init` | ساخت مخزن جدید | Initializes a new repository. |
| `git clone [url]` | کپی کردن مخزن | Clones a repository. |
| `git clone -b [branch] [url]` | کپی کردن یک شاخه خاص | Clones a specific branch of a repository. |

---

# 📤 3) Core Workflow — چرخه کاری اصلی

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git status` | نمایش وضعیت | Shows the status of files. |
| `git add .` | افزودن تمام تغییرات به صف | Stages all current changes. |
| `git commit -m "..."` | ثبت تغییرات | Commits staged changes with a message. |
| `git commit --amend -m "..."` | اصلاح آخرین کامیت | Amends the last commit with a new message. |
| `git push -u origin [branch]` | پوش و تنظیم آپ‌استریم | Pushes and sets the upstream branch. |
| `git pull` | دریافت و ادغام تغییرات | Fetches and merges changes from remote. |
| `git fetch` | فقط دریافت تغییرات (بدون ادغام) | Fetches changes without merging. |

---

# 🌳 4) Branching — کار با شاخه‌ها

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git branch` | نمایش لیست شاخه‌ها | Lists all local branches. |
| `git switch -c [name]` | ساخت و جابجایی به شاخه جدید | Creates and switches to a new branch. |
| `git branch -d [name]` | حذف شاخه ادغام شده | Deletes a merged branch. |
| `git branch -D [name]` | حذف اجباری شاخه | Forcefully deletes a branch. |

---

# 🔗 5) Merging & Rebasing — ادغام و بازآرایی

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git merge [branch]` | ادغام یک شاخه | Merges the specified branch into the current one. |
| `git rebase [branch]` | بازآرایی کامیت‌ها | Re-applies commits from your branch onto another. |
| `git rebase -i HEAD~N` | ریبیس تعاملی (برای ترکیب/ویرایش کامیت‌ها) | Interactively edit or squash the last N commits. |
| `git cherry-pick [commit]` | انتخاب و اعمال یک کامیت خاص | Applies a specific commit from another branch. |

---

# 🕰️ 6) History & Logs — تاریخچه

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git log --oneline --graph` | نمایش تاریخچه فشرده و گرافیکی | Shows a compact, graphical view of history. |
| `git log --author="Name"` | فیلتر تاریخچه بر اساس نویسنده | Filters history by author. |
| `git show [commit]` | نمایش جزئیات یک کامیت | Shows details of a specific commit. |
| `git blame [file]` | نمایش نویسنده هر خط از کد | Shows who last modified each line of a file. |

---

# 🔄 7) Undoing Changes — بازگردانی تغییرات

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git restore [file]` | لغو تغییرات در فایل | Discards changes in a file. |
| `git restore --staged [file]` | خارج کردن فایل از Staging | Unstages a file. |
| `git reset --hard [commit]` | بازنشانی کامل به یک کامیت | Resets to a specific commit, discarding all changes. |
| `git revert [commit]` | ساخت یک کامیت معکوس | Creates a new commit that undoes a previous commit. |

---

# 🧳 8) Stash — ذخیره موقت

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git stash push -m "..."` | ذخیره موقت تغییرات با نام | Temporarily stores changes with a message. |
| `git stash list` | نمایش لیست Stashها | Lists all stashed changes. |
| `git stash pop` | اعمال و حذف آخرین Stash | Applies and removes the last stash. |
| `git stash apply` | اعمال آخرین Stash (بدون حذف) | Applies the last stash but keeps it. |
| `git stash drop` | حذف یک Stash | Deletes a stash from the list. |
| `git stash clear` | حذف تمام Stashها | Deletes all stashes. |

---

# 🌐 9) Remotes — مخازن ریموت

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git remote -v` | نمایش لیست ریموت‌ها | Lists all remote repositories. |
| `git remote add [name] [url]` | افزودن ریموت | Adds a new remote. |
| `git remote set-url [name] [new_url]` | تغییر آدرس یک ریموت | Changes the URL of a remote. |

---

# 📑 10) Advanced Tools — ابزارهای پیشرفته

| دستور (Command) | توضیح فارسی | English Description |
| :--- | :--- | :--- |
| `git worktree add [path] [branch]` | کار روی دو شاخه به طور همزمان | Manages multiple working trees. |
| `git submodule add [url] [path]` | افزودن یک مخزن دیگر به عنوان زیرماژول | Adds another repository as a submodule. |
| `git clean -n` | نمایش فایل‌هایی که حذف خواهند شد | Previews which untracked files would be removed. |
| `git clean -f` | حذف فایل‌های ردگیری نشده (خطرناک!) | Deletes untracked files from the directory. |
| `git bisect start` | شروع عملیات یافتن کامیت معیوب | Starts a binary search to find a faulty commit. |
| `git archive -o [file.zip] HEAD` | خروجی گرفتن از پروژه به صورت فایل فشرده | Creates an archive (e.g., zip) of the project. |

---

# ⚙️ 11) Internal (Plumbing) Commands — دستورات داخلی

Git includes low-level commands for direct repository manipulation, known as "plumbing" (e.g., `hash-object`, `cat-file`, `write-tree`). These are typically used for scripting or deep inspection, not daily work.
گیت شامل دستورات سطح پایینی (مانند `hash-object`, `cat-file`) است که برای دستکاری مستقیم مخزن به کار می‌روند و معمولاً در کارهای روزمره استفاده نمی‌شوند.
