<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>就活に関するアンケート</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        .question {
            margin-bottom: 20px;
        }
        .options {
            margin-left: 20px;
        }
    </style>
</head>
<body>
    <h1>就活に関するアンケート</h1>

    <form>
        <div class="question">
            <h3>1. 企業の何を重視していますか？（複数選択可）</h3>
            <div class="options">
                <input type="checkbox" id="career" name="priority" value="career">
                <label for="career">キャリア</label><br>
                <input type="checkbox" id="training" name="priority" value="training">
                <label for="training">社員育成の制度</label><br>
                <input type="checkbox" id="culture" name="priority" value="culture">
                <label for="culture">社風</label><br>
                <input type="checkbox" id="environment" name="priority" value="environment">
                <label for="environment">労働環境</label><br>
                <input type="checkbox" id="size" name="priority" value="size">
                <label for="size">企業規模</label><br>
                <input type="checkbox" id="info" name="priority" value="info">
                <label for="info">求人情報の情報量</label><br>
                <input type="checkbox" id="philosophy" name="priority" value="philosophy">
                <label for="philosophy">企業理念</label><br>
                <input type="checkbox" id="salary" name="priority" value="salary">
                <label for="salary">給与水準</label><br>
                <input type="checkbox" id="benefits" name="priority" value="benefits">
                <label for="benefits">福利厚生</label><br>
                <input type="checkbox" id="innovation" name="priority" value="innovation">
                <label for="innovation">事業の新規性</label><br>
            </div>
        </div>

        <div class="question">
            <h3>2. どこで就職したいですか？</h3>
            <div class="options">
                <input type="text" id="location" name="location" placeholder="場所を入力してください">
            </div>
            <h4>転勤について：</h4>
            <div class="options">
                <input type="radio" id="no_transfer" name="transfer" value="no_transfer">
                <label for="no_transfer">一切なし</label><br>
                <input type="radio" id="no_transfer_for_now" name="transfer" value="no_transfer_for_now">
                <label for="no_transfer_for_now">当面なし</label><br>
                <input type="radio" id="transfer_ok" name="transfer" value="transfer_ok">
                <label for="transfer_ok">距離に応じて許容</label><br>
            </div>
        </div>

        <div class="question">
            <h3>3. 興味のある業界は何ですか？</h3>
            <div class="options">
                <textarea id="industry" name="industry" rows="4" cols="50"></textarea>
            </div>
        </div>

        <div class="question">
            <h3>4. あなたの情報を教えてください：</h3>
            <div class="options">
                学年：<input type="text" id="grade" name="grade"><br>
                学部：<input type="text" id="faculty" name="faculty"><br>
                性別：
                <select id="gender" name="gender">
                    <option value="male">男性</option>
                    <option value="female">女性</option>
                    <option value="other">その他</option>
                    <option value="prefer_not_to_say">回答しない</option>
                </select>
            </div>
        </div>

        <div class="question">
            <h3>5. 企業SNSではどういった情報を得たいですか？</h3>
            <div class="options">
                <textarea id="sns_info" name="sns_info" rows="4" cols="50"></textarea>
            </div>
        </div>

        <div class="question">
            <h3>6. 就活の情報をどこから得たいですか？</h3>
            <div class="options">
                <textarea id="info_source" name="info_source" rows="4" cols="50"></textarea>
            </div>
        </div>

        <div class="question">
            <h3>7. 就活のスケジュールについて教えてください：</h3>
            <div class="options">
                インターンに行きたい/行った月：<input type="month" id="intern_month" name="intern_month"><br>
                情報収集を行いたい/行った月：<input type="month" id="research_month" name="research_month">
            </div>
        </div>

        <div class="question">
            <h3>8. 企業研究の中で志望企業を決める際に何を特に意識していましたか？</h3>
            <div class="options">
                <textarea id="company_research" name="company_research" rows="4" cols="50"></textarea>
            </div>
        </div>

        <div class="question">
            <h3>9. 時期による就活意識の変化を教えてください：</h3>
            <div class="options">
                就活直前：<textarea id="before_job_hunting" name="before_job_hunting" rows="2" cols="50"></textarea><br>
                就活中：<textarea id="during_job_hunting" name="during_job_hunting" rows="2" cols="50"></textarea><br>
                就活後：<textarea id="after_job_hunting" name="after_job_hunting" rows="2" cols="50"></textarea>
            </div>
        </div>

        <div class="question">
            <h3>10. 実際に情報収集をどこからしていますか/するつもりですか？</h3>
            <div class="options">
                業界に興味を持つ時期：<input type="month" id="industry_interest_month" name="industry_interest_month"><br>
                具体的な会社名や内容を調べる時期：<input type="month" id="company_research_month" name="company_research_month"><br>
                情報源：<textarea id="info_sources" name="info_sources" rows="4" cols="50"></textarea>
            </div>
        </div>

        <div class="question">
            <h3>11. 高校生の方へ：</h3>
            <div class="options">
                就活など将来のことをどのくらい考えていますか？<br>
                <input type="range" id="future_planning" name="future_planning" min="1" max="5"><br>
                大学をいつ頃決めましたか？<input type="month" id="university_decision_month" name="university_decision_month"><br>
                大学を決めた理由：<textarea id="university_reason" name="university_reason" rows="4" cols="50"></textarea>
            </div>
        </div>

        <input type="submit" value="送信">
    </form>
</body>
</html>
