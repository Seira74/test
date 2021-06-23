        <script type="text/javascript">
            function count() {
                var n1 = 3;
                var n2 = 5;
                var nmax = 20 // 最大値
                
                var w1 = 'Fizz'; // 表示ワード1
                var w2 = 'Buzz'; // 表示ワード2
                
                var t = 1200; // 更新インターバル ミリ秒
                
                for (var i=1; i<=nmax+1; i++) with ({i:i}) {
                    
                    setTimeout(function() {
                        
                        if (i == nmax+1) {
                            var str = 'Thank you!';
                        } else if (i % (n1*n2) == 0) { // 公倍数であれば
                            str = w1+w2;
                        } else if (i % n1 == 0) { // n1の倍数であれば
                            str = w1;
                        } else if (i % n2 == 0) { // n2の倍数であれば
                            str = w2;
                        } else {
                            str = i;
                        }
                        document.getElementById('showcase').innerHTML = str;
                    }, i*t
                );
                };
            }
        </script>


課題1の javascriptです。動作は以下のURLでご確認いただけます。<br />
https://gel-extra.tv/test/seira/

一部 stack overflowなどを参照しました。よろしくお願いいたします。
