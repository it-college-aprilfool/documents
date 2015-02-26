# レイアウトの切り替え方

レイアウトを切り替えるにはconfig.rbを編集します。

そのまま例が載ってるので

    # Per-page layout changes:
    #
    # With no layout
    # page "/path/to/file.html", :layout => false
    #
    # With alternative layout
    # page "/path/to/file.html", :layout => :otherlayout
    #
    # A path which all have the same layout
    # with_layout :admin do
    #   page "/admin/*"
    # end

この辺のコメント外してあげればそんな感じで動きます。

(弄るところでいえば :otherlayout とか :admin とかその辺の名前をlayoutディレクトリのファイル名と合わせれば大丈夫ですよ)

### 例

#### /staff/以下にlayouts/staff.erbを適用したい場合

    with_layout :staff do
       page "/staff/*"
    end

#### /index.htmlだけlayouts/top.erbにしたい

    page "/index.html", :layout => :top
