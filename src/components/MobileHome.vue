<template>
  <div class="home-container">
    <div class="headerBox">
      <!-- header -->
      <nav class="navbar navbar-default" role="navigation" style="background:none;border:none;">
      <!-- <nav class="navbar navbar-default navbar-fixed-top" role="navigation" style="background:none;border:none;"> -->
        <div class="container">
            <div class="navbar-header">
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse" style="color:white;border:none;">
                    <span class="sr-only">导航条</span>
                    <span class="icon-bar" style="background: white"></span>
                    <span class="icon-bar" style="background: white"></span>
                    <span class="icon-bar" style="background: white"></span>
                </button>
                <a class="navbar-brand" style="padding: 10px 15px;" href="">
                    <img class="header-logo" src="../assets/mobile/logo.png"/>
                </a>
            </div>
            <div class="collapse navbar-collapse" style="background: rgba(255,255,255,0.8);border:none;text-align:right;position: absolute;width:100%;z-index: 99;">
                <ul class="nav navbar-nav" id="nav-list" style="padding-right:20px;line-height: 40px;width:100%">
                    <!-- <li><span class="nav"><a style="color:#E84142;font-size:16px;font-weight:900;font-family: Calibre-Regular, Calibre;" href="#ecosystem-container">Developers</a></span></li> -->
                    <!-- <li><span class="nav"><a style="color:#E84142;font-size:16px;font-weight:900;font-family: Calibre-Regular, Calibre;" href="#roadmap-container">Whitepaper</a></span></li> -->
                    <li><span class="nav"><a style="color:#E84142;font-size:16px;font-weight:900;font-family: Calibre-Regular, Calibre;" href="#footerAccBox">Community</a></span></li>
                </ul>
            </div>
        </div>
    </nav>
      <div class="header-container">
        <!-- <div class="header-nav">
          <img class="header-logo" src="../assets/mobile/logo.png" alt="logo">
          <img class="header-menu" src="../assets/mobile/menu.png" alt="menu">
        </div> -->

        <div class="header-titles">
          <!-- <div class="header-sub-title">SAMA</div> -->
          <!-- <div class="header-sub-title">Network Service Protocol</div> -->
          <div class="header-title">BUILD A MORE</div>
          <div class="header-title header-redWhite">LIBERTY</div>
          <div class="header-title header-red">SECURE</div>
          <div class="header-title header-redWhite">INCLUSIVE</div>
          <div class="header-title">NETWORK</div>
          <div class="header-sub-title header-sub-titleTop">Provide protection for every user </div>
          <div class="header-sub-title">who enters WEB3.0</div>
        </div>
        <div class="header-content">
          <!-- <div class="header-item">
            <img class="header-item-icon" src="../assets/mobile/vision.png" alt="">
            <div class="header-note">
              <div class="header-item-title">
                Vision
              </div>
              <div class="header-item-content">
                Access protocols unimpeded links to Internet users around the world
              </div>
            </div>
          </div>
          <div class="header-item">
            <img class="header-item-icon" src="../assets/mobile/mission.png" alt="">
            <div class="header-note">
              <div class="header-item-title">
                Mission
              </div>
              <div class="header-item-content">
                Support the efficient operation of web2 & web3 applications, data privacy and security
              </div>
            </div>
          </div> -->
          <div class="header-building">
            Start Building
            <img class="header-building-icon" src="../assets/right.png" alt="右箭头">
            <!-- coming soon -->
          </div>
        </div>
        <!-- <div class="header-defense"></div> -->
      </div>
    </div>
    <!-- features -->
    <!-- <div class="feature-container">
      <div class="feature-title">FEATURES</div>
      <div class="feature-menu">
        <div :class="`feature-nav ${item.id == currentFeature? 'active': ''}`" v-for="item in features" :key="item.id" @click="changeFeautre(item)">
          <img class="feature-icon" :src="item.icon" />
          <div class="feature-name">{{ item.name }}</div>
        </div>
      </div>
      <div class="feature-content">
        <div class="text" v-for="item in features.filter(item => item.id == currentFeature)[0].contents" :key="item">
          <span class="keyword">{{ item.name }}</span>
          {{ item.content }}
        </div>
      </div>
    </div> -->
    <!-- WHY SAMA PROTOCOL -->
    <div class="mobileProBox">
      <div class="mobileProTitle">
        WHY<br/> SAMA PROTOCOL
      </div>
      <div class="mobileProItemBox">
        <div :class="['mobileProItem',proItem.isMouse==true?'mobileProItemHover':'']" v-for="(proItem,proIndex) in protocolRowList" :key="proIndex" @click="protocolRowFunc(proItem)">
          <img v-if='proItem.isMouse == false' :src='proItem.src1' alt="" class="mobileProItemImg"/>
          <img v-if='proItem.isMouse == true' :src='proItem.src2' alt="" class="mobileProItemImg"/>
          <div v-if='proItem.isMouse == true' :class="['mobileProItemContent mobileProItemContent'+Number(proIndex+1)]">
            <!-- {{ proItem.content }} -->
          </div>
        </div>
      </div>
    </div>
    <!-- ecosystem 模块 -->
    <div class="ecosystem-container" id="ecosystem-container">
      <div class="eco-padding eco-title model_title_width">Ecosystem</div>
      <div class="eco-padding eco-sub-title">process</div>
      <img class="eco-padding eco-image" src="../assets/mobile/ecosystem.png" alt="">
      <div class="eco-padding eco-item">SAMA consists of <strong>SE community BaaS</strong> and</div>
      <div class="eco-padding eco-item"><strong>network security protocols</strong></div>
      <div class="eco-padding eco-item">( Avalanche subnet、Router&Server network、</div>
      <div class="eco-padding eco-item">SDK&API）</div>
    </div>
    <!-- ecological -->
    <div class="ecologic-container">
      <div class="logic-title-box">
        <div class="eco-padding logic-title model_title_width">Ecologic</div>
        <div class="eco-padding logic-sub-title model_title_width2">Economic cycle</div>
      </div>
      <img class="eco-padding logic-image" src="../assets/mobile/ecological.png" alt="">
      <div class="eco-padding logic-note">The self-organizing and structured network embeds</div>
      <div class="eco-padding logic-note">the blockchain's incentive model,network and</div>
      <div class="eco-padding logic-note">economy to form the dual circulation of the SAMA</div>
      <div class="eco-padding logic-note">protocol</div>
      <!-- <div class="eco-padding logic-note">The self-organizing and structured network embeds the blockchain's incentive model, network and economy to form the dual circulation of the SAMA protocol</div> -->
    </div>
    <!-- network -->
    <div class="ecosystem-container" id="ecosystem-container">
      <div class="eco-padding eco-title model_title_width">Maker</div>
      <div class="eco-padding eco-sub-title">Community</div>
      <img class="eco-padding eco-image" src="../assets/mobile/ecosystemTwo.png" alt="">
      <div class="eco-padding eco-item">Protect the works of creators and give a safe and free network environment</div>
      <div class="eco-padding eco-item">Do not change the user's habits, dual web dual mirroring</div>
      <div class="eco-padding eco-item">Token + point system</div>
    </div>
    <!-- team -->
    <!-- <div class="team-container">
      <div class="team-title">TEAM</div>
      <div class="team-items">
        <div class="team-item" v-for="item in teams" :key="item.id">
          <div class="team-item-header">
            <div class="team-avatar">
              <img :src="item.avatar" alt="">
            </div>
            <div class="team-group">
              <div class="team-name">{{ item.name }}</div>
              <div class="team-role">{{ item.role }}</div>
            </div>
          </div>
          <div class="team-item-content">
            {{ item.description }}
          </div>
        </div>
      </div>
    </div> -->
    <!-- advisor -->
    <!-- <div class="advisor-container">
      <div class="advisor-title">ADVISOR</div>
      <div class="advisor-items">
        <div class="advisor-item" v-for="item in advisors" :key="item.id">
          <div class="advisor-item-header">
            <div class="advisor-avatar">
              <img :src="item.avatar" alt="">
            </div>
            <div class="advisor-group">
              <div class="advisor-name">{{ item.name }}</div>
              <div class="advisor-role">{{ item.role }}</div>
            </div>
            <img class="adviser-arrow" @click="toggleAdviser(item)" v-if="!item.show" src="../assets/mobile/downarrow.png" />
            <img class="adviser-arrow" @click="toggleAdviser(item)" v-else src="../assets/mobile/uparrow.png" />
          </div>
          <div class="advisor-item-content" v-show="item.show">
            {{ item.description }}
          </div>
        </div>
      </div>
    </div> -->
    <!-- roadmap -->
    <div class="roadmap-container" id="roadmap-container">
      <div class="road-title">ROADMAP</div>
      <!-- <div class="road-content" v-for="item in roadmaps" :key="item">
        <div class="road-left">
          <span v-if="item.name">{{ item.name }}</span>
          <div class="road-node" v-else></div>
        </div>
        <div v-if="!item.name" class="road-line"></div>
        <div class="road-line2" v-if="item.success"></div>
        <div class="road-line3" v-else></div>
        <div :class="`road-right ${!item.name? 'border': ''}`">{{ item.content }}</div>
      </div> -->
      <div class="road-contentImg">
        <img src="../assets/mobile/roadImg.png" alt=""/>
      </div>
    </div>
    <!-- associ -->
    <div class="associ-container">
      <div class="associ-title">In Association With</div>
      <div class="friend-groups">
        <!-- <img src="../assets/footerOne.png" alt="">
        <img src="../assets/footerTwo.png" alt="">
        <img src="../assets/footerThree.png" alt="">
        <img src="../assets/footerFour.png" alt="">
        <img src="../assets/footerFive.png" alt=""> -->
        <img src="../assets/footerFiveHezuo.png" alt="">
      </div>
      <!-- <div class="associ-group">
        <div class="associ-item">MUTE</div>
        <div class="associ-item">Jump</div>
        <div class="associ-item">Goldentree</div>
      </div> -->
      <div class="footerAccBox" id="footerAccBox">
        <div class="associ-join-icon">
          <img src="../assets/mobile/contact.png" alt="">
        </div>
        <div class="associ-join">Join SAMA Community</div>
        <div class="associ-contact-group">
          <div class="associ-contact-item" v-for="(communItem,communIndex) in communityList" :key="communIndex">
            <div class="associ_left">
              <img :src="communItem.src" alt="" class="associ-contact-icon" />
              <div>
                <a :href="communItem.link" target="_blank">{{ communItem.name }}</a>
              </div>
            </div>
            <div class="associ_right">
              >
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- footer -->
    <div class="footer-container">
      <img src="../assets/logo2.png" class="footer-logo" alt="">
      <!-- <div class="footer-item">Developers</div> -->
      <!-- <div class="footer-item">Whitepaper</div> -->
      <div class="footer-item">Community</div>
    </div>
    <!-- copyright -->
    <div class="copyright">
      Copyright © 2022 SAMA.NET All rights reserved.
    </div>
  </div>
</template>
<script>
import avatar from '@/assets/avatar.jpg'
import userIcon from '@/assets/users.png'
import privacyIcon from '@/assets/privacy.png'
import combinationIcon from '@/assets/combination.png'

export default {
  name: 'MobileHomePage',
  props: {
    msg: String
  },
  data() {
    return {
      currentFeature: 1,
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
          show: true,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        },
        {
          id: 2,
          name: 'gknmoon2',
          role: 'co-founder',
          avatar: avatar,
          show: false,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        },
        {
          id: 3,
          name: 'gknmoon3',
          role: 'co-founder',
          avatar: avatar,
          show: false,
          description: 'Graduated from Northwest University, MSC Apex core geometry developer, distributed database developer, delivery director of TOP Network high-performance sharding public chain project, director of MOAC public chain application ecology construction, director of TAFChain project&pre research, one of the original authors of Tenon network'
        }
      ],
      features: [
        {
          id: 1,
          icon: userIcon,
          name: 'Massive users',
          contents: [
            {
              'name': 'Low cost:',
              'content': 'Any idle server equipment and bandwidth traffic can join the network as nodes to provide services, while benefiting from the low cost of behavior on the Avalanche subnet user chain'
            },
            {
              'name': 'High throughput:',
              'content': 'The child chain built by the Avalanche Avalanche subnet provides dual network node mapping and settlement, and the dual network provides secure and private data transmission'
            },
          ]
        },
        {
          id: 2,
          icon: privacyIcon,
          name: 'Security and privary',
          contents: [
            {
              'name': 'Protect security and privacy:',
              'content': 'The network built on the blockchain account model and consensus mechanism transmits data to protect user and data security and privacy'
            },
            {
              'name': 'Censorship-resistant, single-point failure-resistant: ',
              'content': 'Distributed, multi-centralized nodes form a network cluster to prevent centralized blockade'
            },
          ]
        },
        {
          id: 3,
          icon: combinationIcon,
          name: 'Combination & High scalability',
          contents: [
            {
              'name': 'Composable:',
              'content': 'Benefiting from the composability of Avalanche main and subnet users, the coin holding user and application user groups are highly integrated'
            },
            {
              'name': 'High scalability:',
              'content': 'The network cluster composed of self-organizing discrete distributed nodes can continuously provide network security services and promote each other with the scale of application users'
            },
          ]
        }
      ],
      roadmaps: [
        {
          'name': '2022 Q3',
          'content': 'SN privacy protocol dual network (Router&Server Network) Core function development completed',
          'success': true
        },
        {
          'name': "",
          'content': `Genesis Rules     Forfeiture rule
            Access rules    Voting rules
            Role reward rules  Governance rules
            …`,
          'success': true
        },
        {
          'name': '2022 Q4',
          'content': `Official, white paper&deck completed
                Dual network compatible avalanche subnet
                Economic model&implementation of governance mechanism`,
          'success': false
        },
        {
          'name': '2023 Q1',
          'content': `SDK&API encapsulation
            Subnet browser of SN privacy protocol
            Wallet development
            Test the online cable`,
          'success': false
        },
        {
          'name': '2023 Q2',
          'content': `SN privacy protocol code audit
              Open source code in succession
              Main network online`,
          'success': false
        },
        {
          'name': '',
          'content': `Web2 & Web3 App cooperation;
              Provide corresponding tool chain development to facilitate B end Build application`,
          'success': false
        }
      ],
      isMenuShow:false,
      protocolRowList:[
        {
          title:'ONE-CLICK SHARING',
          content:'any content can be injected to SAMA with one-click sharing',
          isMouse:true,
          src1:require('../assets/mobile/proto7b.png'),
          src2:require('../assets/mobile/proto7a.png'),
        },
        {
          title:'DOUBLE MIRROR',
          content:"don't change user's habits, web2&web3 dual mirroring",
          isMouse:false,
          src1:require('../assets/mobile/proto6b.png'),
          src2:require('../assets/mobile/proto6a.png'),
        },
        {
          title:'LOW GAS',
          content:'the gas fee is 0.01 SAMA not AVAX',
          isMouse:false,
          src1:require('../assets/mobile/proto1b.png'),
          src2:require('../assets/mobile/proto1a.png'),
        },
        {
          title:'HIGHT THROUGHPUT',
          content:'an independent AVAX subnet',
          isMouse:false,
          src1:require('../assets/mobile/proto2b.png'),
          src2:require('../assets/mobile/proto2a.png'),
        },
        {
          title:'Unlimited access web3',
          content:'protect creators’ works and provide the unlimited network',
          isMouse:false,
          src1:require('../assets/mobile/proto8b.png'),
          src2:require('../assets/mobile/proto8a.png'),
        },
        {
          title:'SECURE',
          content:'multiple encryption to protect data transmission',
          isMouse:false,
          src1:require('../assets/mobile/proto4b.png'),
          src2:require('../assets/mobile/proto4a.png'),
        },
        {
          title:'PRIVACY',
          content:'internet data transmission privacy',
          isMouse:false,
          src1:require('../assets/mobile/proto5b.png'),
          src2:require('../assets/mobile/proto5a.png'),
        },
        {
          title:'HIGHT SCALABILITY',
          content:'self-organizing distributed nodes form network clusters',
          isMouse:false,
          src1:require('../assets/mobile/proto3b.png'),
          src2:require('../assets/mobile/proto3a.png'),
        },
      ],
      communityList:[
          {
            src:require('../assets/github.png'),
            link:'https://github.com/samanetwork',
            name:'Github'
          },
          {
            src:require('../assets/twitter.png'),
            link:'https://twitter.com/sama_network',
            name:'Twitter'
          },
          {
            src:require('../assets/telegram.png'),
            link:'https://t.me/+TDotfcLSPjdhYTg1',
            name:'Telegram'
          },
          {
            src:require('../assets/discord.png'),
            link:'https://discord.gg/Ahju7jCz',
            name:'Discord'
          }
        ],
    }
  },
  methods: {
    changeFeautre(item) {
      // console.log(item);
      if (this.currentFeature !== item.id) {
        this.currentFeature = item.id
      }
    },
    toggleAdviser(item) {
      item.show = !item.show
    },
    menuEnter(){
      // console.log(1)
      this.isMenuShow = !this.isMenuShow
    },
    menumOut(){
      this.isMenuShow = false
    },
    protocolRowFunc(item){
      for(let i in this.protocolRowList){
        if(this.protocolRowList[i].title == item.title){
          this.protocolRowList[i].isMouse = true
          item.isMouse = true
        }else{
          this.protocolRowList[i].isMouse = false
        }
      }
    }
  }
}
</script>
<style scoped>
  @import url('../css/mobile.css');
  html, body {
    width: 100vh;
    height: 100vh;
    overflow: hidden;
  }
  a {
    text-decoration: none;
  }
</style>