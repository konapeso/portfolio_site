<template>
  <div id="app">
    <v-app id="inspire">
      <v-card max-width="800" class="mx-auto" ma-3>
        <v-container>
          <h2 　class="mt-10">ACTIVITY</h2>

          <v-row dense>
            <v-col v-for="(item, i) in items" :key="i" cols="12">
              <a :href="item.link">
                <v-hover
                  v-slot:default="{ hover }"
                  :open-delay="hover.openDelay"
                  :close-delay="hover.closeDelay"
                  :disabled="hover.disabled"
                  :value="hover.value"
                >
                  <v-card :elevation="hover ? 8 : 2" color="grey lighten-5">
                    <div class="d-flex flex-row mb-6">
                      <v-avatar class="ma-4" size="150" tile>
                        <v-img :src="item.img"></v-img>
                      </v-avatar>
                      <div>
                        <v-card-title class="subtitle-1 font-weight-medium" v-text="item.title"></v-card-title>

                        <v-card-title class="subtitle-1 text-left" v-text="item.article"></v-card-title>

                        <v-card-subtitle class="float-left" v-text="item.subtitle"></v-card-subtitle>
                      </div>
                    </div>
                  </v-card>
                </v-hover>
              </a>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </v-app>
  </div>
</template>

<style scoped>
.v-application--wrap {
  background-color: #fff;
}
a {
  text-decoration: none;
}
h2 {
  margin-bottom: 50px;
}
.container{
  margin-top:100px;
}
</style>

<script>
export default {
  data() {
    return {
      hover: [
        {
          disabled: false,
          openDelay: "0",
          closeDelay: "0",
          value: false
        }
      ],
      items: [
        {
          img: "/item1.png",
          title: "世界を歩いてきた2人がラジオを始めるための作戦会議",
          subtitle: "2019/4",
          article:
            "幅広い視点から沖縄を説くラジオ番組を持ちたいゆとり世代の2人が毎週違うテーマをもとにライブ配信をしながらディスカッションしていました。",
            link: "https://www.facebook.com/marimo.oshiro/posts/1972543952843488"
        },
        {
          img: "/item2.png",
          title: "KOZA de 朝活 ",
          subtitle: "2019/5",
          article:
            "毎週水曜日早朝、ネイティブスピーカーと一緒に英会話を行っています。 ディープで国際色豊かなコザの町で、楽しく英語に触れてみませんか？",
          link: "https://www.instagram.com/morning_meetup_koza/"
        },
        {
          img: "/item3.png",
          title: "IVS 2019 in Summer",
          subtitle: "2019/7",
          article:
            "無限の可能性を持つベンチャー企業を生み出す場・集まる場」を創出する。という理念で立ち上げられた、国内外の経営者・経営幹部を主な対象とした招待制カンファレンスにスタッフとして参加しました。",
          link: "https://www.facebook.com/konami.ota.73/posts/317408209142583"
        },
        {
          img: "/item4.png",
          title: "イベント資金をクラウドファンディングで調達",
          subtitle: "2019/8",
          article:
            "沖縄の若手アーティスト・クリエイターが充分に才能を発揮できる機会をつくるため、クラウドファンデングでイベントの資金調達を行いました。",
          link: "https://camp-fire.jp/v2/projects/172242"
        },
        {
          img: "/item9.png",
          title: "琉球新報朝刊に掲載",
          subtitle: "2019/9",
          article:
            "zele+ vol.1イベントについて琉球新報さんから取材を受けました。",
          link: "https://ryukyushimpo.jp/news/entry-985012.html"
        },
        {
          img: "/item6.png",
          title: "zele+ vol.1 開催",
          subtitle: "2019/9",
          article:
            "沖縄県出身のクリエイター・アーティストを集め、インタラクティブなイベントの企画・運営を行い、100名以上のお客様にお越しいただきました。",
          link: "https://www.facebook.com/konami.ota.73/posts/352445938972143"
        },
        {
          img: "/item7.png",
          title: "Startup Weekend Okinawa Vol.9",
          subtitle: "2019/9",
          article:
            "全世界各国の週末の三日間を使った企業体験プログラムでデザイナー・エンジニアとして参加し、チームで無料で旅行ができ、自分のスキルを活かして社会に貢献できるサービスをつくり、3位入賞を果たしました。",
          link: "https://www.facebook.com/konami.ota.73/posts/356775525205851"
        },
        {
          img: "/item8.png",
          title: "Rails Girls Okinawa 2nd",
          subtitle: "2019/10",
          article:
            "プログラミングのワークショップを宜野湾ベイサイド情報センターで10/4(金), 5(土)に開催させていただきました。",
          link:
            "http://www.railsgirls.com/okinawa-2nd.html?fbclid=IwAR3WQ5dLAydibUnltWPGt8uHjWm2s9Wy0ECNQ1t_-dPrc3_ONyvv06pktcM"
        }
      ]
    };
  }
};
</script>>