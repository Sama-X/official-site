<template>
  <div class="home-container">
    <!-- <div class="row">
      <div class="col-xs-6 col-md-3">
        <a href="#" class="thumbnail">
          12
        </a>
      </div>
      <div class="col-xs-6 col-md-3">
        <a href="#" class="thumbnail">
          34
        </a>
      </div>
    </div> -->
    <div class="header-container">
      <div class="header-menu">
        <div class="header-left">
          <img class="logo" src="../assets/logo.png" alt="logo">
        </div>
        <div class="header-right">
          <!-- <span class="nav"><a href="#team-container">Developers</a></span> -->
          <!-- <span class="nav"><a href="#roadmap-container">Whitepaper</a></span> -->
          <span class="nav"><a href="#footer">Community</a></span>
          <span class="nav button">
            en
            <span class="icon"></span>
          </span>
        </div>
      </div>
      <div class="header-content">
        <div class="left-content">
          <div class="title2">
            <!-- SAMA Network Service -->
          </div>
          <div class="title">BUILD A MORE</div>
          <div class="title_boder">
            <div class="titleRed">
              LIBERTY
            </div>
            <div class="titleWhite">
              SECURE
            </div>
            <div class="titleRed">
              INCLUSIVE
            </div>
          </div>
          <div class="title">NETWORK</div>
          <div class="title2 title2_topMargin">Provide protection for every user who enters WEB3.0</div>
          <div class="building">
            Start Building
            <img src="../assets/right.png" alt="right">
            <!-- coming soon -->
          </div>
        </div>
        <div class="right-content">
          <!-- <img src="../assets/channel.png" alt="suiidao"> -->
        </div>
      </div>
    </div>
    <div class="protocolBox">
      <div class="protocolHeaderTitle">
        WHY SAMA PROTOCOL
      </div>
      <div class="protocolRow">
        <div :class="['protocolImg protocolImg'+(proIndex+1), proItem.isMouse==true ? 'protocolImghover'+(proIndex+1) : '']" v-for="(proItem,proIndex) in protocolRowList" :key="proIndex" @mouseenter="promouseEnter(proItem)" @mouseout="promousemOut(proItem)">
          <!-- <div :class="['protocolTitle',proItem.isMouse==true?'protocolTitleHover':'']" @mouseenter="promouseEnter(proItem)" @mouseout="promousemOut(proItem)">
            {{ proItem.title }}
          </div> -->
          <div :class="['protocolContent pContent'+(proIndex+1),proItem.isMouse==true?'protocolContentHover':'']">
            <!-- {{ proItem.content }} -->
          </div>
        </div>
      </div>
    </div>
    <div class="ecosystem-container">
      <div class="eco-left">
        <div class="eco-title">
          <div class="eco-keyword">Ecosystem</div>
          <div class="eco-keyword eco-keyword-nobackground">process</div>
        </div>
        <!-- <div class="eco-sub-title">
          SAMA consists of SE community BaaS and
        </div> -->
        <div class="eco-content">
          SAMA consists of SE community BaaS and
        </div>
        <div class="eco-content">
          network security protocols （ Avalanche subnet、
        </div>
        <div class="eco-content">
          Router&Server network、SDK&API）
        </div>
      </div>
      <div class="eco-right">
        <img src="../assets/ecosystem.png" alt="">
      </div>
    </div>
    <div class="ecological-container">
      <div class="logic-left">
        <img src="../assets/ecological.png" alt="">
      </div>
      <div class="logic-right">
        <div class="logic-title">Ecological</div>
        <div class="logic-sub-title">Economic Cycle</div>
        <div class="logic-content">The self-organizing and structured network</div>
        <div class="logic-content">embeds the blockchain's incentive model,</div>
        <div class="logic-content">network and economy to form the dual</div>
        <div class="logic-content">circulation of the SAMA protocol.</div>
      </div>
    </div>
    <div class="ecosystem-container ecosystem2">
      <div class="eco-left">
        <div class="eco-title">
          <div class="eco-keyword">Maker</div>
          <div class="eco-keyword eco-keyword-nobackground">Community</div>
        </div>
        <!-- <div class="eco-sub-title">
          SAMA consists of SE community BaaS and
        </div> -->
        <div class="eco-content">
          Protect the works of creators and give a safe and free network environment
        </div>
        <div class="eco-content">
          Do not change the user's habits, dual web dual mirroring
        </div>
        <div class="eco-content">
          Token + point system
        </div>
      </div>
      <div class="eco-right">
        <img src="../assets/ecosystemTwo.png" alt="">
      </div>
    </div>
    <div class="roadmap-container" id="roadmap-container">
      <div class="road-title">ROADMAP</div>
      <div class="roadmap">
        <img src="../assets/histroy.png" alt="">

        <!-- <div class="road-content road-contentOne">
          SN privacy protocol dual network<br/>
          (Router&Server Network)<br/>
          Core function development completed
        </div>
        <div class="road-content road-contentTwo">
          Genesis Rules<br/>
          Access rules<br/>
          Role reward rules<br/>
          Forfeiture rule<br/>
          Voting rules<br/>
          Governance rules<br/>
          …
        </div>
        <div class="road-content road-contentThree">
          The official website, project introduction and<br/>
          other documents have been completed; the<br/>
          dual-network integration avalanche subnet<br/>
          builds a sub-chain to realize the<br/>
          encapsulation of the interface
        </div>
        <div class="road-content road-contentFour">
          Community construction, economic model and<br/>
          governance mechanism implementation,<br/>
          complete link testing, wallet, browser, community<br/>
          BaaS product prototype construction, SAMA test<br/>
          network online
        </div>
        <div class="road-content road-contentFive">
          Protocol code audit, code open source,<br/>
          SAMA mainnet online, community BaaS<br/>
          products online
        </div>
        <div class="road-content road-contentSix">
          Continue to develop<br/>
          tool chain products and<br/>
          service web2 content to<br/>
          move into SAMA web3<br/>
          community products to<br/>
          promote the<br/>
          development of trade<br/>
          unions for makers
        </div> -->
      </div>
    </div>
    <div class="association-container">
      <div>In Association With</div>
    </div>
    <div class="friends-conainer">
      <div class="friend-groups">
        <!-- <img src="../assets/footerOne.png" alt="">
        <img src="../assets/footerTwo.png" alt="">
        <img src="../assets/footerThree.png" alt="">
        <img src="../assets/footerFour.png" alt="">
        <img src="../assets/footerFive.png" alt=""> -->
        <img src="../assets/footerFiveHezuo.png" alt="">

      </div>
      <div class="friend-contact">
        <div class="contact-left">
          <img src="../assets/contact.png" alt="">
          <div class="contact-note">Join our community</div>
          <!-- <div class="contact-right-arrow">></div> -->
        </div>
        <div class="contact-right">
          <div class="contact_box">
            <div class="contact_boxLeft">
              <img src="../assets/github.png" alt="" class="contact-icon" />
              <div>
                <a href="https://github.com/samanetwork" target="_blank">Github</a>
              </div>
            </div>
            <div class="contact_boxRight">
              >
            </div>
          </div>
          <div class="contact_box">
            <div class="contact_boxLeft">
              <img src="../assets/twitter.png" alt="" class="contact-icon" />
              <div>
                <a href="https://twitter.com/sama_network" target="_blank">Twitter</a>
              </div>
            </div>
            <div class="contact_boxRight">
              >
            </div>
          </div>
          <div class="contact_box">
            <div class="contact_boxLeft">
              <img src="../assets/telegram.png" alt="" class="contact-icon" />
              <div>
                <a href="https://t.me/+TDotfcLSPjdhYTg1" target="_blank" rel="noopener noreferrer">Telegram</a>
              </div>
            </div>
            <div class="contact_boxRight">
              >
            </div>
          </div>
          <div class="contact_box">
            <div class="contact_boxLeft">
              <img src="../assets/discord.png" alt="" class="contact-icon" />
              <div>
                <a href="https://discord.gg/Ahju7jCz" target="_blank" rel="noopener noreferrer">Discord</a>
              </div>
            </div>
            <div class="contact_boxRight">
              >
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-container" id="footer">
      <div class="footer">
        <div class="footer-left">
          <img src="../assets/logo2.png" alt="">
        </div>
        <div class="footer-right">
          <div class="right-note">
            <!-- <div>Developers</div> -->
            <!-- <div>Whitepaper</div> -->
            <div>Community</div>
          </div>
          <div class="right-link">
            <a href="https://twitter.com/sama_network" target="_blank">Twitter</a>
          </div>
          <div class="right-link">
            <a href="https://t.me/+TDotfcLSPjdhYTg1" target="_blank" rel="noopener noreferrer">Telegram</a>
          </div>
          <div class="right-link">
            <a href="https://discord.gg/Ahju7jCz" target="_blank" rel="noopener noreferrer">Discord</a>
          </div>
        </div>
      </div>
      <div class="footer-line"></div>
      <div class="footer-copyright">
        Copyright © 2022 SAMA.NET All rights reserved.
      </div>
    </div>
  </div>
</template>

<script>
import avatar from '@/assets/avatar.jpg'
export default {
  name: 'HomePage',
  props: {
    msg: String
  },
  data() {
    return {
      teams: [
        {
          id: 1,
          name: 'gknmoon',
          role: 'founder',
          avatar: avatar,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        },
        {
          id: 2,
          name: 'gknmoon2',
          role: 'co-founder',
          avatar: avatar,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        },
        {
          id: 3,
          name: 'gknmoon3',
          role: 'co-founder',
          avatar: avatar,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        },
        {
          id: 4,
          name: 'gknmoon4',
          role: 'co-founder',
          avatar: avatar,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        }
      ],
      advisors: [
        {
          id: 1,
          name: 'gknmoon',
          role: 'founder',
          avatar: avatar,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        },
        {
          id: 2,
          name: 'gknmoon2',
          role: 'co-founder',
          avatar: avatar,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        },
        {
          id: 3,
          name: 'gknmoon3',
          role: 'co-founder',
          avatar: avatar,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        }
      ],
      protocolRowList:[
        {
          title:'ONE-CLICK SHARING',
          content:'any content can be injected to SAMA with one-click sharing',
          isMouse:true,
        },
        {
          title:'DOUBLE MIRROR',
          content:"don't change user's habits, web2&web3 dual mirroring",
          isMouse:false,
        },
        {
          title:'LOW GAS',
          content:'The gas fee is 0.01 SAMA not AVAX',
          isMouse:false,
        },
        {
          title:'HIGHT THROUGHPUT',
          content:'an independent AVAX subnet',
          isMouse:false,
        },
        {
          title:'Unlimited access web3',
          content:'protect creators’ works and provide the unlimited network',
          isMouse:false,
        },
        {
          title:'SECURE',
          content:'multiple encryption to protect data transmission',
          isMouse:false,
        },
        {
          title:'PRIVACY',
          content:'internet data transmission privacy',
          isMouse:false,
        },
        {
          title:'HIGHT SCALABILITY',
          content:'self-organizing distributed nodes form network clusters',
          isMouse:false,
        },
      ],
      numberA:'',
    }
  },
  methods:{
    promouseEnter(item){
      // console.log(item)
      for(let i in this.protocolRowList){
        if(item.title == this.protocolRowList[i].title){
          this.protocolRowList[i].isMouse = true
          item.isMouse = true
        }else{
          this.protocolRowList[i].isMouse = false
        }
      }
      // console.log(item)
    },
    promousemOut(){
      // this.numberA = ''
      // for(let i in this.protocolRowList){
      //   if(item.title == this.protocolRowList[i].title){
      //     // this.protocolRowList[i].isMouse = true
      //     // item.isMouse = true
      //     this.numberA = i
      //   }
      // }
      //     this.protocolRowList[this.numberA].isMouse = true
      // console.log(this.numberA,'this.numberA')
      // console.log(this.protocolRowList,'this.protocolRowList')
      // this.$forceUpdate()
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import url('../css/compute.css');
</style>
