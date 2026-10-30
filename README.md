![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=intecs2609ap03-prog&theme=github_dark)
![](https://streak-stats.demolab.com?user=intecs2609ap03-prog&theme=github_dark)

# お気に入りのHTMLひな型
```json
{
  "Bootstrap5 Dark Simple Template": {
    "prefix": "!!!",
    "body": [
      "<!DOCTYPE html>",
      "",
      "<html data-bs-theme=\"dark\">",
      "  <head>",
      "    <meta charset=\"UTF-8\">",
      "    <title>Title</title>",
      "    <!-- #region CDNインポート -->",
      "    <!-- bootstrap -->",
      "    <link href=\"https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css\" rel=\"stylesheet\" integrity=\"sha384-sRIl4kxILFvY47J16cr9ZwB07vP4J8+LH7qKQnuqkuIAvNWLzeN8tE5YBujZqJLB\" crossorigin=\"anonymous\">",
      "    <script src=\"https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js\" integrity=\"sha384-FKyoEForCGlyvwx9Hj09JcYn3nv7wiPVlz7YYwJrWVcXK/BmnVDxM+D2scQbITxI\" crossorigin=\"anonymous\" defer></script>",
      "    ",
      "    <!-- Animate.css -->",
      "    <link rel=\"stylesheet\" href=\"https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css\"/>",
      "    <!-- #endregion -->",
      "  </head>",
      "",
      "  <body>",
      "    <div class=\"animate__animated animate__fadeInUp\">",
      "      <h3 style=\"text-align: center; margin-top: 150px; font-size: 100px;\">HelloWorld!!</h3>",
      "    </div>",
      "  </body>",
      "</html>"
    ],
    "description": "オレオレHTMLひな型"
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

