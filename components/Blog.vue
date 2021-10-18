<template>
  <section id="Blog" class="pt-120 pb-90 top-shape">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-12">
          <!-- section title -->
          <div class="title">最新貼文</div>
          <!-- End of section title -->
        </div>
      </div>
      <div class="row">
        <div class="col-md-6 col-lg-4" v-for="blog in blogs" :key="blog.title">
          <!-- single blog inner -->
          <div class="single-blog-inner">
            <!-- blog image -->
            <!-- <div class="post-image">
              <a href="#">
                <img src="/assets/img/blog/blog1.png" alt="" />
              </a>
              <div class="post-date">
                <p><span>30</span>Sep</p>
              </div>
            </div> -->
            <!--End of  blog image -->

            <!-- post content -->
            <div class="post-content">
              <div class="post-details">
                <div class="post-title">
                  <h3>
                    <a target="_blank" :href="blog.link">{{ blog.title }}</a>
                  </h3>
                </div>
                <p v-for="paragraph in blog.content" :key="paragraph">
                  {{ paragraph }}
                </p>
                <a target="_blank" :href="blog.link"
                  ><i class="fa fa-arrow-circle-o-right"></i>More</a
                >
              </div>
              <!-- <div class="post-info d-flex">
                <a href="#"><span>By</span>Admin</a>
                <a href="#"><span>2</span> Comeent</a>
              </div> -->
            </div>
            <!-- End of post content -->
          </div>
          <!-- End of single blog inner -->
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Blog',
  data() {
    return {
      blogs: [
        {
          title:
            '想儲外幣可以點儲？想提早10年去外地退休🍹？想退休之後每個月仲有一萬蚊被動收入💰？',
          link:
            'https://www.facebook.com/moneysheephk/photos/a.107043131724842/119998390429316',
          content: [
            '皇牌多元外幣理財計劃複利滾存，你值得擁有🤗港幣🇭🇰、英鎊🇬🇧、美元🇺🇸、澳元🇦🇺、加元🇨🇦、人民幣🇨🇳通通都可以自由轉換💞總能符合你需要！'
          ]
        },
        {
          title: '#理財news 大家最近係咪都陸逐收到 #綠色炸彈 呢🍏？',
          link:
            'https://www.facebook.com/moneysheephk/photos/a.107043131724842/119339840495171',
          content: [
            '又係時候審視一下自己有無搵專家幫你睇下點樣減低殺傷力🔫～ 立即Whatsapp登記📩領取至抵扣稅方案！'
          ]
        },
        {
          title: '#理財433',
          link:
            'https://www.facebook.com/moneysheephk/photos/a.107043131724842/119020173860471/',
          content: [
            '近年為咗保持身材坊間有「168、204」等減肥斷食法，其實投資理財上都有一個黃金比例4:3:3，即40% 30% 30% 的百分比分配在「投資📈」、「儲蓄🐷」和「日常開支👛」上。如果你自認不善理財，或者害怕承受風險而不敢投資，你可以度身訂造一個適合自己的投資理財黃金比例，一定可以幫到你。',
            '#立即聯絡 我們幫你打造屬於你嘅投資理財黃金比例💛！'
          ]
        },
        {
          title: '你50歲後的人生是如何🤔？',
          link:
            'https://www.facebook.com/moneysheephk/photos/a.107043131724842/117767237319098/',
          content: [
            '50歲好多人都覺得人生過左大半場，結婚👰🏻🤵🏻、生仔👶🏻、買樓🏠、仔女出身👩🏻‍🎓👨🏻‍🎓、湊埋孫👨‍👧‍👦，好似已成定局。但係50歲只係一個數字，絕對唔係一個限制。50歲先能夠將過往所累積嘅經驗同智慧，應用係現在同未來。#50歲更加要投資 好好善用手頭上嘅資源，過一個更豐盛嘅第二人生！'
          ]
        },
        {
          title: '究竟星座唔同性格會對應返邊種理財策略？👀',
          link: 'https://www.facebook.com/moneysheephk/posts/118330467262775',
          content: [
            '風象星座：「我愛冒險，鍾意新鮮刺激既事物😜」',
            '#雙子座♊️、#天秤座♎️、#水瓶座♒️既朋友轉數快又鍾意刺激，較進取的基金投資選擇啱晒佢哋口味！',
            '水象星座：「我鍾意細心聆聽同分析，平衡各方需要，照顧人夠晒全面🤗」',
            '#巨蟹座♋️、#天蠍座♏️、#雙魚座♓️既朋友最樂於助人，分析仔細得嚟又穩打穩紮，按比例分散投資最啱佢地，中短線派息型基金+中長線儲蓄計劃 Fit晒！',
            '土象星座：「我係穩陣派，最緊要保本🤓」',
            '#金牛座♉️、#處女座♍️、#山羊座♑️既朋友投資方案注重安全性，穩中求勝、善用時間坡度長遠複利滾存既保本儲蓄計劃最適合！',
            '火象星座：「我直腸直肚，夠膽衝又夠膽玩，藝高人膽大🤑」',
            '#白羊座♈️、#獅子座♌️、#射手座♐️既朋友性格直率但有時未免過於衝動，多元資產派息型基金投資進可攻，退可守，仲可以按需要隨時靈活轉換，最啱做火象星座既緩衝！'
          ]
        },
        {
          title: '圓規之下，圓滿做好規劃！',
          link:
            'https://www.facebook.com/moneysheephk/photos/a.107043131724842/118049453957543',
          content: [
            '打風係不能預料嘅風險，一早去超市買定食物日用品，就同係平時做好 #理財 規劃一樣，將來預到任何突如其來嘅風險來襲都應付有餘～😎立即聯絡我地理財專家幫你規劃一下！'
          ]
        },
        {
          title: '你50歲後的人生是如何🤔？',
          link:
            'https://www.facebook.com/moneysheephk/photos/a.107043131724842/117767237319098/',
          content: [
            '50歲好多人都覺得人生過左大半場，結婚👰🏻🤵🏻、生仔👶🏻、買樓🏠、仔女出身👩🏻‍🎓👨🏻‍🎓、湊埋孫👨‍👧‍👦，好似已成定局。但係50歲只係一個數字，絕對唔係一個限制。50歲先能夠將過往所累積嘅經驗同智慧，應用係現在同未來。#50歲更加要投資 好好善用手頭上嘅資源，過一個更豐盛嘅第二人生！'
          ]
        },
        {
          title: '【香港人迷思】🏠 一定要買樓先叫人生贏家？',
          link:
            'https://www.facebook.com/moneysheephk/photos/a.107043131724842/116467517449070',
          content: [
            '如果買樓係自住、結婚或者係用來做身份象徵的話，其實樓價點升點跌都會買樓。但如果唔係上述情況，物業投資係現時係咪仲好似以前咁有潛在回報🤔？',
            '🔹過去10年樓價每年只有10厘升幅，比起幾十年前以幾何倍數升值簡直蚊比同牛比',
            '🔹每年出租回報只有2厘，都未計管理費、維修費等雜費成本，仲有可能有租霸事件或變凶宅等不可控風險',
            '🔹QE左咁耐，環球央行收水或令未來會加息，減少市場資金的流動性，買樓收租成本就更加高',
            '🔹物業別種資產一啲都唔Liquid，因為想套部份現個陣唔可以淨係賣走個廚房或厠所，而賣物業亦唔係咁容易找到買家即Trade，仲有印花稅、律師費成本，一覺唔覺意加息後收租都唔夠供Mortgage',
            '所以，周不時見到有業主平手或損手離場唔出奇🤷🏻‍♀️。至於有筆資金係手，仲有啲咩出路？即管問下我地點樣懶洋洋都可以將資產Upgrade😎🍹！'
          ]
        },
        {
          title: '富人之路！機會來了！',
          link: 'https://www.facebook.com/moneysheephk/photos/115885894173899',
          content: [
            '周圍借稅貸都低息，富人一直都會襯低息善用自己Credit去進行槓杆，套出資金去賺息差！簡單講本金減返個平息都淨賺高達10厘💵💵💵！仲唔快啲向我地查詢襯機會踏上呢條富人之路！'
          ]
        },
        {
          title: '香港地 今時今日100萬可以買咩？',
          link: 'https://www.facebook.com/moneysheephk/photos/115869137508908',
          content: [
            '🔸 車位？NO！無200-300萬都唔洗諗啦！',
            '🔸 樓？更加NO！100萬唔好玩啦，納米樓首期都俾唔起',
            '🔸 車？終於YES！but...要供要養又要維修又大食🔥 燒錢之選',
            '#100萬增值出路與其擺係銀行蝕息蝕通脹，不如放係穩陣嘅平台月月收息仲Happy啦～🤗🎉'
          ]
        },
        {
          title: '一層物業 #Double收租又收息',
          link: 'https://www.facebook.com/moneysheephk/photos/115648647530957',
          content: [
            '供左層樓幾年，仲有空間再按揭？善用物業活化釋放額度，懶羊羊夫婦再教埋你點樣每月收租又收息！實行將資產快速Double Up!'
          ]
        }
      ]
    };
  }
};
</script>

<style scoped>
.title {
  font-size: 50px;
  text-align: center;
  margin-bottom: 80px;
  font-family: 'genJyuuGothic-bold';
}
</style>
