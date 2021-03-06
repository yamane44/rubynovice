# Rubynovice

Ruby programming mastering platform using Github.

情報共有環境であるGithubを使って，Rubyのprogrammingを習得することを目指しています．

## インストール法
- githubで自分のアカウントにdaddygongon/rubynoviceをforkする
- 自分のPCにcloneする

## 使用法
- 自分の好きな名前(daddy)をつけたディレクトリーを作る．
- "./lib/daddy/ex_files.rb"を準備
- ex_files.rbにrequire "ex1"を書く
- class Rubynoviceに解答を保存していく．
- 書き方は./lib/daddy/ex1_classified.rbを参照のこと．
- rspecで，個人ごとの検査を実行するには
  - 環境変数RUBYNOVICE_NAMEにディレクトリー名を入れる
    - (csh,tcsh)setenv RUBYNOVICE_NAME daddy
    - (bash,zsh)export RUBYNOVICE_NAME=daddy
  - rspec spec/ex2_spec.rb
  - 失敗したとこで止める
    - 'rspec spec/ex2_spec.rb  --fail-fast'
    - rake spec hogehogeとかでもOKだが動作不安定．
    - 複数の検査を一度に処理しようとするときに前のclassが生き残っている？

```ruby
bob% cat lib/daddy/ex_files.rb
#require "ex1_1"
require "ex1_classified"
require "ex2_classified"
```

```ruby
bob% cat lib/daddy/ex1_classified.rb 
class Rubynovice

  def ex1_1
    return "hello world.\n"
  end

  def ex1_2
    return 1+1
  end

  def ex1_3
    ans = 1+1
    text = sprintf("ans=%i\n",ans)
    return text
  end


end
```

## 課題
### Githubではリンク切れ，wikiのSidebarから辿れ

### 入門課題
1. [ex1(gets puts)](file.ex1.html)
1. [ex2(loop)](file.ex2.html)
1. [ex3(array)](file.ex3.html)
1. [ex4(if)](file.ex4.html)
1. [ex5(method)](file.ex5.html)

### 発展課題
1. [ex_prime](file.ex_prime.html)
1. [ex_GoogleRecruit](file.ex_GoogleRecruit.html)
