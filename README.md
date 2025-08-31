# GitHub Desktop, GitHub Gists ve GitHub Copilot

## GitHub Desktop Nedir?
<p align="justify">Git ve GitHub işlemlerini grafik arayüz (GUI) üzerinden yapmanızı sağlayan, masaüstü uygulamasıdır.<br>
<b>Kime Hitap Eder?</b> Özellikle yeni başlayanlar veya komut satırı (CLI) kullanmak istemeyenler için idealdir.<br>
<b>Ne Yapar?</b>
<li>Repo oluşturma, clone'lama,</li>
<li>Branch oluşturma,</li>
<li>Commit oluşturma,</li>
<li>Push/Pull/Merge işlemleri,</li>
<b>Avantajı:</b> Komutları ezberlemeden, tıklamalarla kolayca Git işlemleri yapabilirsiniz.</p>

[Github Desktop Sayfası Linki](https://desktop.github.com/download/) ilgili sayfadan GitHub Desktop'ı indirip adımları takip ederek kurulum yapabilirsiniz.

![Github Desktop Görüntü](https://github.com/cyasar34/Git-vs-Github/blob/main/repository_olusturma.jpg)

### En Basit Haliyle: "Proje Dosyaları için Google Drive"

<p align="justify">GitHub'ı, yazılım projelerinize özel bir Google Drive veya Dropbox gibi düşünebilirsiniz. Ancak çok daha akıllı ve güçlüdür:
<li>Sadece dosyaları saklamaz, her değişikliğin geçmişini de kaydeder.</li>
<li>Aynı dosya üzerinde aynı anda çalışan insanların çakışmasını (conflict) yönetir.</li>
<li>Kodları incelemeye, hata bildirmeye, tartışmaya olanak tanır.</li>

### Neden GitHub Kullanmalıyız?

<li align="justify"><b> Güvenli Bulut Yedekleme:</b> Kodunuz ve tüm versiyon geçmişi bulutta saklanır. Bilgisayarınız bozulsa bile projeniz güvendedir.</li>

<li align="justify"><b> Zaman Makinesi:</b> Projenizin eski haline istediğiniz an dönebilir, kimin ne değişiklik yaptığını görebilirsiniz.</li>

<li align="justify"><b> Kolay İş Birliği: </b> Aynı proje üzerinde, aynı anda, dünyanın her yerinden ekip arkadaşlarınızla sorunsuzca çalışabilirsiniz.</li>

<li align="justify"><b> Proje Yönetimi: </b> Görev takibi (Issues), kod incelemesi (Pull Request) ve proje tahtaları (Projects) ile her şey organize olur.</li>

<li align="justify"> <b> Otomasyon (CI/CD): </b> Kodunuzu gönderdiğinizde testlerin otomatik çalışmasını ve sunucuya otomatik yüklenmesini sağlarsınız.</li>

<li align="justify"><b> Portfolyo & CV: </b> Hesabınız, işverenlere gösterdiğiniz canlı bir yetenek portfolyosudur. </li>

<li align="justify"> <b>Açık Kaynak Katkı: </b> Dünyadaki en büyük yazılım projelerine katkıda bulunmanın en kolay yoludur. </li>

### GitHub Terminolojisi

#### Repository (Repo) / Depo

<p align="justify">Projenizin tüm dosyalarının, klasör yapısının ve bu dosyalardaki tüm değişiklik geçmişinin (commit'lerin) saklandığı yerdir.
<em>Projenizin için özel bir "klasör" ya da "proje dosyası" gibi düşünebilirsiniz.</em> Ancak bu klasör, dosyalarınızın yanı sıra yaptığınız her değişikliğin de kaydını tutan akıllı bir zaman makinesi gibidir.<br>
Türleri:
<li>Yerel (Local) Repo: Bilgisayarınızın hard disk'inde bulunur.</li>
<li>Uzak (Remote) Repo: GitHub, GitLab gibi bir bulut sunucusunda bulunur.</li><br>
<em>Kısacası: Repository, projenizin tamamıdır.</em>

#### Branch (Dal)

<p align="justify"> Projenizin farklı versiyonlarını veya farklı özelliklerini birbirinden bağımsız ve paralel olarak geliştirmenizi sağlayan bir hat.<br> 
Bir ağacın ana gövdesi (main branch) vardır. Siz yeni bir özellik üzerinde çalışmaya başladığınızda, bu gövdeden yeni bir dal (branch) oluşturursunuz. Ana gövdeyi bozmadan, risksiz bir şekilde daldaki çalışmanızı bitirirsiniz. İşiniz bittiğinde, bu dalı ana gövdeye birleştirirsiniz (merge).<br>
<em>Kısacası: Branch, projenizin içinde açılmış paralel ve bağımsız bir çalışma alanıdır.</em>

#### Clone (Klonlama)

<p align="justify">Bir uzak depoyu (örneğin, GitHub'daki bir projeyi) tüm versiyon geçmişiyle birlikte kendi bilgisayarınıza kopyalama işlemidir.
<em> git clone "repo-url" komutuyla yapılır.</em>
Bir dosyayı buluttan (Google Drive) kendi bilgisayarınıza indirmek gibidir.<br>
<em>Kısacası: Clone ile bilgisayarına indirirsin.</em>

#### Fork (Çatallama)

<p align="justify">Bir başkasının GitHub'daki reposunu kendi GitHub hesabınıza kopyalamaktır. GitHub arayüzündeki "Fork" butonuna tıklanarak yapılır. Bir belgeyi alıp "Farklı Kaydet" diyerek kendi adınızla kaydetmek gibidir. <br>
<em>Kısacası: Fork ile GitHub hesabına kopyalarsın.</em>

#### Main (Ana Dal)

<p align="justify">Bir projedeki ana, kararlı ve çalışan sürümün bulunduğu varsayılan branch'tir (dal). Eskiden master olarak adlandırılırdı. <br>
<em>Kısacası:Main projenin ana gövdesidir. </em>

#### Pull (Çekme)

<p align="justify">Uzak depodaki (GitHub'daki) güncel değişiklikleri kendi yerel deponuza indirme işlemidir. Ekip çalışmasında, başkalarının yaptığı değişikliklerle yerel reponuzu güncel tutmak için.<br>
<b>Komut: git pull</b><br>
<em>Kısacası: Pull/Push senkronizasyon içindir.</em>

#### Push (İtme)

<p align="justify">Yerel deponuzdaki commit'leri uzak depoya (GitHub'a) gönderme işlemidir. Yaptığınız değişiklikleri diğer ekip üyeleriyle paylaşmak veya yedeklemek için.<br>
<b>Komut: git push</b><br>
<em>Kısacası: Pull/Push senkronizasyon içindir.</em>

#### Merge (Birleştirme)

<p align="justify">İki dalı (branch) birleştirme işlemidir. Bir özellik branch'inde yapılan değişiklikleri ana dala (main) eklemek için. Bir repository üzerinde bulunan bir branch'in başka bir branch ile birleştirilme işlemidir.<br>
<em>Kısacası: Merge birleştirme içindir.</em>

#### Conflict (Çakışma)

<p align="justify">Aynı dosyanın aynı satırında, farklı kişiler tarafından yapılan ve Git'in otomatik olarak birleştiremediği değişiklikler. Manuel olarak müdahale edip hangi değişikliklerin kalacağına karar vermeniz gerekir. Örneğin, iki kişi aynı Word belgesinin aynı yerini farklı şekilde düzenlerse çakışma olur.<br>
<em>Kısacası: Conflict iki kodun çakışmasıdır çözülmesi gereken sorundur.</em>

#### Pull Request (PR) / Merge Request (MR)

<p align="justify">Bir branch'deki değişiklikleri, ana branch'e birleştirme talebi göndermektir. Kod incelemesi (code review) yapılması, tartışılması ve test edilmesi için bir mekanizma sağlar. <br>
<em>Kısacası: Pull Request ise iş birliği ve kalite kontrol mekanizmasıdır.</em>

#### Stash (Geçici Saklama)

<p align="justify">Henüz commit etmediğiniz değişiklikleri geçici olarak bir kenara saklamanızı sağlar. Aniden başka bir branch'e geçmeniz gerektiğinde veya acil bir düzeltme yapmanız gerektiğinde, yarım kalan işinizi kaybetmeden saklarsınız.<br>
<b>Komutlar:
<li>git stash → Değişiklikleri saklar.</li>
<li>git stash pop → Saklanan değişiklikleri geri yükler.</li></b><br>
<em>Kısacası: Stash askıya alma işlemidir.</em>

#### Discard (Atma)

<p align="justify">Commit edilmemiş değişiklikleri tamamen iptal etmek, dosyayı son commit haline geri döndürmek. Yaptığınız değişikliklerden memnun değilseniz ve baştan başlamak isterseniz.<br>
<b>Komut: 
<li>git restore "dosya-adi"</li>  
<li>git checkout --"dosya-adi"</li></b><br>
<em>Kısacası: Discard iptal etme işlemidir.</em>

#### Remote (Uzak)

<p align="justify">Projenizin bulut sunucusunda (örn. GitHub, GitLab) bulunan kopyası. Ekip çalışması, yedekleme ve projeyi dağıtım için merkezi bir depo görevi görür.<b>origin</b> genelde projenizin GitHub'daki ana uzak deposunu ifade eder.<br>
<em>Kısacası: Remote bulut işlevi görür.</em>

#### Local (Yerel)

<p align="justify">Projenizin kendi bilgisayarınızda bulunan kopyası. Geliştirme yapmak, test etmek ve değişiklikleri commit etmek için kullanırsınız.<br>
<em>Kısacası: Local sizin makineniz işlevi görür.</em>

## Bu Github paylaşımının IEEE ve APA formatlarınada atıf verilme şekli:
- IEEE--> C. Yasar, "GitHub-Terminolojisi" GitHub, [Online]. Erişim Linki: https://github.com/cyasar34/GitHub-Terminolojisi Son Erişim Tarihi: Gün Ay Yıl.
- APA--> Yasar, C. (2024). GitHub-Terminolojisi[GitHub Deposu]. GitHub. Erişim Linki: https://github.com/cyasar34/GitHub-Terminolojisi Son Erişim Tarihi: Gün Ay Yıl.
  
> **Proje Durumu:** İlgili dokümanların paylaşımı ders kapsamında gerçekleştirilmiştir. GitHub bölümünden beğeni bildirimi olarak bir yıldız vererek çalışmalarımı destekleyebilirsiniz. <br>
> **Katkıda Bulunma:** Dokümanlarınızda kullanılacaksanız ilgili atıf yöntemlerini kullanmanız ve haber vermeniz çok önemlidir. <br>
> **Lisans:** MIT Lisansı altında yayımlandı.  



# GitHub Terminology

## What is GitHub?
<p align="justify"><b>Git,</b> is like a time machine that takes a “snapshot” (commit) of every stage of your project and allows you to return to those snapshots at any time.  <b>GitHub</b> is a social platform where you can upload these photo albums to the cloud, share them with others, and edit them together.</p>
<p align="justify"><b>Git,</b> is a version control system. It runs on your local computer. It works via the command line.<br>
<b>GitHub on the other hand,</b> is a service and website that allows you to store your Git repositories in the cloud (on the internet). In other words, it acts as a “host” for your Git repository.</p>

### In a Nutshell: “Google Drive for Project Files”

<p align="justify">Think of GitHub as a Google Drive or Dropbox specifically for your software projects. But it's much smarter and more powerful:
<li>It doesn't just store files; it also records the history of every change.</li>
<li>It manages conflicts when multiple people work on the same file at the same time.</li>
<li>It allows you to review code, report bugs, and discuss issues.</li>

### Why Should We Use GitHub?

<li align="justify"><b> Secure Cloud Backup:</b> our code and all version history are stored in the cloud. Even if your computer crashes, your project is safe.</li>

<li align="justify"><b> Time Machine:</b> You can revert your project to its previous state at any time and see who made what changes.</li>

<li align="justify"><b> Easy Collaboration: </b> ou can work seamlessly with your teammates on the same project, at the same time, from anywhere in the world.</li>

<li align="justify"><b> Project Management: </b> Everything is organized with task tracking (Issues), code review (Pull Request), and project boards (Projects).</li>

<li align="justify"> <b> Automation (CI/CD): </b> When you submit your code, tests run automatically and are automatically deployed to the server.</li>

<li align="justify"><b> Portfolio & CV:  </b> Your account is a live showcase of your skills for employers.</li>

<li align="justify"> <b> Open Source Contributions: </b> It's the easiest way to contribute to the world's largest software projects. </li>

### GitHub Terminology

#### Repository (Repo)

<p align="justify">This is where all your project files, folder structure, and the entire change history (commits) for these files are stored.
<em>You can think of it as a special “folder” or “project file” for your project.</em> However, this folder is like a smart time machine that keeps track of every change you make, in addition to your files.<br>
Types:
<li>Local Repo: Located on your computer's hard drive.</li>
<li>Remote Repo: Located on a cloud server such as GitHub or GitLab.</li><br>
<em>In short: The repository is your entire project.</em>

#### Branch

<p align="justify"> A line that allows you to develop different versions or different features of your project independently and in parallel.<br> 
A tree has a main trunk (main branch). When you start working on a new feature, you create a new branch from this trunk. You complete your work on the branch without disturbing the main trunk and without any risk. When you are done, you merge this branch back into the main trunk.<br>
<em>In short: A branch is a parallel and independent workspace within your project.</em>

#### Clone 

<p align="justify">BCloning is the process of copying a remote repository (for example, a project on GitHub) to your own computer, along with its entire version history.
<em> It is done with the command git clone “repo-url”.</em>
It is similar to downloading a file from the cloud (Google Drive) to your own computer.<br>
<em>In short: With clone, you download it to your computer.</em>

#### Fork

<p align="justify">Copying someone else's GitHub repository to your own GitHub account. This is done by clicking the “Fork” button on the GitHub interface. It's like taking a document and saving it under your own name by clicking “Save As.” <br>
<em>In short: You copy it to your GitHub account with Fork.</em>

#### Main

<p align="justify">The default branch where the main, stable, and working version of a project is located. It used to be called master.  <br>
<em>In short: Main is the main body of the project. </em>

#### Pull

<p align="justify">The process of downloading the latest changes from the remote repository (GitHub) to your local repository. In team work, this is to keep your local repository up to date with changes made by others.<br>
<b>Command: git pull</b><br>
<em>In short: Pull/Push is for synchronization.</em>

#### Push (Pushing)

<p align="justify">The process of sending commits from your local repository to the remote repository (GitHub). This is done to share your changes with other team members or to back them up.<br>
<b>Command: git push</b><br>
<em>In short: Pull/Push is for synchronization.</em>

#### Merge

<p align="justify">The process of combining two branches. To add changes made in a feature branch to the main branch. It is the process of merging one branch in a repository with another branch.<br>
<em>In short: Merge is for combining.</em>

#### Conflict

<p align="justify">Changes made by different people to the same line of the same file that Git cannot merge automatically. You must manually intervene and decide which changes to keep. For example, if two people edit the same part of the same Word document differently, a conflict occurs.<br>
<em>In short: Conflict is a problem that needs to be solved when two codes clash.</em>

#### Pull Request (PR) / Merge Request (MR)

<p align="justify">It is a request to merge the changes in a branch into the main branch. It provides a mechanism for code review, discussion, and testing.  <br>
<em>In short: Pull Request is a collaboration and quality control mechanism.</em>

#### Stash (Temporary Storage)

<p align="justify">Allows you to temporarily save changes you haven't committed yet. If you suddenly need to switch to another branch or make an urgent fix, you can save your unfinished work without losing it.<br>
<b>Commands:
<li>git stash → Saves changes.</li>
<li>git stash pop → Restores saved changes.</li></b><br>
<em>In short: Stash is a suspension process.</em>

#### Discard

<p align="justify">Completely discards uncommitted changes, reverting the file to its last committed state. Use this if you are unhappy with your changes and want to start over.<br>
<b>Commands: 
<li>git restore “file-name”</li>  
<li>git checkout --“file-name”</li></b><br>
<em>In short: Discard is the undo operation.</em>

#### Remote 

<p align="justify">The copy of your project located on your cloud server (e.g., GitHub, GitLab). It serves as a central repository for teamwork, backup, and project distribution. <b>origin</b> usually refers to your project's main remote repository on GitHub.<br>
<em>In short: Remote functions as your cloud.</em>

#### Local

<p align="justify">The copy of your project located on your own computer. You use it for development, testing, and committing changes.<br>
<em>In short: Local functions as your machine.</em>

## How to cite this GitHub post in IEEE and APA formats:
- IEEE--> C. Yasar, "GitHub-Terminolojisi" GitHub, [Online]. Erişim Linki: https://github.com/cyasar34/GitHub-Terminolojisi Son Erişim Tarihi: Gün Ay Yıl.
- APA--> Yasar, C. (2024). GitHub-Terminolojisi[GitHub Deposu]. GitHub. Erişim Linki: https://github.com/cyasar34/GitHub-Terminolojisi Son Erişim Tarihi: Gün Ay Yıl.
  
> **Project Status:** The relevant documents have been shared as part of the course. You can support my work by giving it a star as a like notification on the GitHub section. <br>
> **Contributions:** If you plan to use these documents, it is very important that you use the appropriate citation methods and notify me. <br>
> **License:** Published under the MIT License.







