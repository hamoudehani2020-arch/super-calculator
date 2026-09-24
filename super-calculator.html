<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الآلة الحاسبة الخارقة</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
        }

        body {
            background: #11141a;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            padding: 15px;
        }

        .container {
            background: #1a1e29;
            border: 2px solid #333a4d;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.7);
            max-width: 450px;
            width: 100%;
            padding: 20px;
        }

        /* عنوان واضح وكبير بالتاء المربوطة */
        .title {
            text-align: center;
            font-size: 1.8rem;
            font-weight: bold;
            color: #00d2d3;
            margin-bottom: 15px;
        }

        /* شاشة بأرقام ضخمة وواضحة للرؤية */
        .display {
            background: #000;
            border-radius: 12px;
            padding: 15px 20px;
            margin-bottom: 15px;
            text-align: left;
            word-break: break-all;
            direction: ltr;
            border: 2px solid #282f44;
        }

        .prev-op {
            min-height: 24px;
            color: #8892b0;
            font-size: 1.2rem;
        }

        .curr-op {
            font-size: 2.8rem;
            font-weight: bold;
            color: #00f2fe;
        }

        .buttons {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 10px;
        }

        button {
            border: none;
            outline: none;
            background: #282e3f;
            color: #fff;
            font-size: 1.4rem;
            font-weight: bold;
            padding: 16px 5px;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.15s;
        }

        button:active {
            transform: scale(0.96);
        }

        /* زر الحذف بالعربي - بارز وواضح */
        button.btn-del {
            background: #e74c3c;
            color: #fff;
            font-size: 1.4rem;
        }

        button.btn-clear {
            background: #d63031;
        }

        button.btn-ten {
            background: #6c5ce7;
            font-size: 1.5rem;
        }

        button.btn-inf {
            background: #0984e3;
            font-size: 1.8rem;
        }

        button.btn-inc {
            background: #00b894;
            color: #fff;
            font-size: 1.4rem;
        }

        button.op {
            background: #e67e22;
            font-size: 1.6rem;
        }

        button.equal {
            background: #2ecc71;
            font-size: 1.8rem;
        }

        button.special {
            background: #34495e;
            color: #00d2d3;
        }
    </style>
</head>
<body>

<div class="container">
    <div class="title">الآلة الحاسبة الخارقة</div>

    <div class="display">
        <div id="prevOp" class="prev-op"></div>
        <div id="currOp" class="curr-op">0</div>
    </div>

    <div class="buttons">
        <!-- الصف 1 -->
        <button class="btn-clear" onclick="clearAll()">AC</button>
        <button class="btn-del" onclick="deleteDigit()">حذف</button>
        <button class="btn-inc" title="زيادة آخر رقم بمقدار 1" onclick="incrementLast()">+1</button>
        <button class="op" onclick="setOp('/')">÷</button>

        <!-- الصف 2 -->
        <button class="btn-ten" onclick="insertVal('10')">10</button>
        <button class="btn-inf" onclick="insertVal('Infinity')">∞</button>
        <button class="special" onclick="insertVal(Math.PI.toFixed(2))">π</button>
        <button class="op" onclick="setOp('*')">×</button>

        <!-- الصف 3 -->
        <button onclick="insertVal('7')">7</button>
        <button onclick="insertVal('8')">8</button>
        <button onclick="insertVal('9')">9</button>
        <button class="op" onclick="setOp('-')">-</button>

        <!-- الصف 4 -->
        <button onclick="insertVal('4')">4</button>
        <button onclick="insertVal('5')">5</button>
        <button onclick="insertVal('6')">6</button>
        <button class="op" onclick="setOp('+')">+</button>

        <!-- الصف 5 -->
        <button onclick="insertVal('1')">1</button>
        <button onclick="insertVal('2')">2</button>
        <button onclick="insertVal('3')">3</button>
        <button class="special" onclick="applySquare()">x²</button>

        <!-- الصف 6 -->
        <button onclick="insertVal('0')">0</button>
        <button onclick="insertVal('.')">.</button>
        <button class="special" onclick="applySqrt()">√</button>
        <button class="equal" onclick="compute()">=</button>
    </div>
</div>

<script>
    let current = '0';
    let previous = '';
    let operation = null;
    let resetNext = false;

    const currOp = document.getElementById('currOp');
    const prevOp = document.getElementById('prevOp');

    function update() {
        currOp.innerText = current;
        if (operation) {
            let symbol = operation === '*' ? '×' : (operation === '/' ? '÷' : operation);
            prevOp.innerText = `${previous} ${symbol}`;
        } else {
            prevOp.innerText = '';
        }
    }

    function insertVal(val) {
        if ((current === '0' && val !== '.') || resetNext) {
            current = '';
            resetNext = false;
        }
        if (val === '.' && current.includes('.')) return;
        current += val;
        update();
    }

    // زر الحذف الذي يحذف آخر رقم مدخل
    function deleteDigit() {
        if (current === 'Infinity' || current === '-Infinity' || current.length <= 1) {
            current = '0';
        } else {
            current = current.slice(0, -1);
        }
        update();
    }

    // زر +1 لزيادة آخر رقم
    function incrementLast() {
        if (current === 'Infinity' || current === '-Infinity') return;
        let num = parseFloat(current);
        if (!isNaN(num)) {
            current = (num + 1).toString();
        }
        update();
    }

    function setOp(op) {
        if (current === '') return;
        if (previous !== '') compute();
        operation = op;
        previous = current;
        resetNext = true;
        update();
    }

    function compute() {
        let res;
        const p = parseFloat(previous);
        const c = parseFloat(current);
        if (isNaN(p) || isNaN(c)) return;

        switch (operation) {
            case '+': res = p + c; break;
            case '-': res = p - c; break;
            case '*': res = p * c; break;
            case '/': res = (c === 0) ? 'Infinity' : p / c; break;
            default: return;
        }

        current = res.toString();
        operation = null;
        previous = '';
        resetNext = true;
        update();
    }

    function applySquare() {
        const n = parseFloat(current);
        current = (n * n).toString();
        update();
    }

    function applySqrt() {
        const n = parseFloat(current);
        current = (n >= 0) ? Math.sqrt(n).toString() : '0';
        update();
    }

    function clearAll() {
        current = '0';
        previous = '';
        operation = null;
        update();
    }
</script>

</body>
</html>

