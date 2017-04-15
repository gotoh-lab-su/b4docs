# 卒業研究関係文書管理フォルダ

## 方針

コンピュータの中にばらばらにファイルを格納しているのは良くないので一ヶ所にまとめて管理する。ただし、ソフトウェアのソースファイルなどは個別にリポジトリを作って管理する方が便利なので、この管理フォルダの中には含めない。

一ヶ所にまとめておけば、デバイス間（たとえば研究室のPCと自宅のPCの間など）で簡単に卒業研究関係文書を共有できる。

## フォルダ一覧
- Docs: 卒業論文を除く、メモや覚書などの文書
- PPTs: 発表スライド
- Refs: 収集した論文や資料
- Theses: 卒業論文のソースファイル、画像ファイルなど

## Gitの使い方について

- [Linux/Unix環境でのGit入門](http://www.aise.ics.saitama-u.ac.jp/~gotoh/IntroGitOnLinux.html)
- [TortoiseGitのインストール方法](http://www.aise.ics.saitama-u.ac.jp/~gotoh/HowToInstallTortoiseGit.html)：Windows環境でのGitクライアント

## 後藤研究室の学生の最初の操作

GitLabにリポジトリを作成してみてください。
0. 上述のLinuxおよびWindowsでのGitを使用できる環境を整える
1. [GitLabの使い方](http://www.aise.ics.saitama-u.ac.jp/~gotoh/HowToUseGitLab.html)の「公開鍵の登録」（Linux環境およびWindows環境のそれぞれで必要）を行う
2. このリポジトリをクローンする。Windows環境の場合は[Gitでのクローンのやり方](http://www.aise.ics.saitama-u.ac.jp/~gotoh/HowToCloneOnGit.html)にしたがう。Linuxの場合は、以下のように行う。
   ```
   % cd
   % git clone https://github.com/gotoh-lab-su/b4docs.git
   % cd b4docs
   % git remote -v
   ```
3. GitLab上に自分用リモートリポジトリを作成する。[
プロジェクトの新規作成](http://www.aise.ics.saitama-u.ac.jp/~gotoh/CreateNewProjectOnGitLab.html)の「プロジェクトの作成」にしたがい、リモートリポジトリを作成する。次に「既にGitでソースコードを管理していた場合」にしたがって、クローンしたフォルダのリモートリポジトリのURLを新しく作成したGitLabのリモートリポジトリに書き換える。
4. その後、Pushする

