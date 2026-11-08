![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=intecs2609ap03-prog&theme=github_dark)
![](https://streak-stats.demolab.com?user=intecs2609ap03-prog&theme=github_dark)

# お気に入りのHTMLひな型
```json
{
  "HTML Boilerplate with Dark CSS": {
    "prefix": "!!!",
    "body": [
      "<!DOCTYPE html>",
      "",
      "<html>",
      "    <head>",
      "        <meta charset=\"UTF-8\">",
      "        <title>${1:Document}</title>",
      "        <!-- #region style -->",
      "        <style>",
      "            :root {",
      "                --primary-background: #121214;",
      "                --primary-text: #ededed;",
      "                --secondary-background: #1a1a1e;",
      "                --secondary-text: #9ba1a6;",
      "                --card-background: #21212646;",
      "            }",
      "",
      "            body {",
      "                background-color: var(--primary-background);",
      "                color: var(--primary-text);",
      "            }",
      "",
      "            .card {",
      "                background-color: var(--card-background);",
      "                border-radius: 10px;",
      "                backdrop-filter: blur(10px);",
      "                margin: 1px;",
      "                padding: 1px;",
      "            }",
      "",
      "            .large-content {",
      "                text-align: center; ",
      "                margin-top: 150px; ",
      "                font-size: 100px;",
      "                padding: 50px;",
      "            }",
      "        </style>",
      "        <!-- #endregion -->",
      "    </head>",
      "",
      "    <body>",
      "        <div class=\"large-content card\">",
      "            <p>${2:Hello World!!!}</p>",
      "        </div>",
      "    </body>",
      "</html>",
      "$0"
    ],
    "description": "ダークテーマのスタイルとカードコンポーネントを含むHTMLのテンプレート"
  }
}
```
# お気に入りのPHPフロントコントローラー用ひな型
```json
{
  "Single Front Controller": {
    "prefix": "fctrl",
    "body": [
      "//シングルフロントコントローラー",
      "\\$requestMethod = \\$_SERVER['REQUEST_METHOD'];",
      "if (\\$requestMethod !== 'GET' && \\$requestMethod !== 'POST') ",
      "    clientError(\"本システムではGET/POST以外対応していません。\");",
      "",
      "\\$path = null;",
      "if (\\$requestMethod === 'GET') \\$path = \\$_GET['path'] ?? null; ",
      "else if (\\$requestMethod === 'POST') \\$path = \\$_POST['path'] ?? null;",
      "",
      "if (is_null(\\$path)) ClientErrorAcction(\"pathクエリ/パラメータが指定されていません。\");",
      "else if (\\$path === \"home\") HomeAction();",
      "",
      "function ClientErrorAcction(\\$errorMsg) {",
      "    //クライアントエラー用のページを表示してください。",
      "}",
      "",
      "function HomeAction() {",
      "    //初期ページを表示してください。",
      "}"
    ],
    "description": "シングルフロントコントローラーの基本構造"
  }
}
```

