<template>
  <div class="info">
  </div>
</template>

<script>
export default {
  data () {
    return {
      leftPart: [
        {
          text: '基本信息', 
          color: '#eb7d04', 
          type: 1, 
          info:[
            {img:1 , context:'1997/03/04'},
            {img:2 , context:'159 5711 8442'},
            {img:3, context:'harveyzhq@vip.qq.com'},
            {img:4, context:'中国·浙江·杭州'}
          ]
        },
        {
          text: '技能特长', 
          color: '#92b630', 
          type: 2, 
          title:'技能：', 
          sum: 5, 
          info:[
            {topic:'前端技术', count: 5, color: '#34a6d1'},
            {topic:'Office', count: 4, color: '#e6a906'},
            {topic:'C++', count: 3, color: '#92b630'},
            {topic:'Photoshop', count: 3, color: '#e86c6c'}
          ]
        },
        {
          text: '框架熟悉程度', 
          color: '#e86c6c',
          type: 3, 
          sum: 7,
          info:[
            {topic:'Vue',count: 6,color: '#34a6d1'},
            {topic:'Bootstrap',count: 5,color: '#e6a906'},
            {topic:'JQuery',count: 5,color: '#92b630'},
            {topic:'Node.js',count: 4,color: '#e86c6c'}
          ]
        },
        {
          text: '兴趣爱好', 
          color: '#6396a9',
          type: 4,
          info:[
            'static/images/5.png',
            'static/images/6.png',
            'static/images/7.png'
          ]
        }
      ],
      rightPart: [
        {
          text: 'SELF EVALUATION 自我评价',
          color: '#eb7d04',
          context: [
            {
              type: 1,
              title: '学习背景：',
              text: [
                '拥有浙江工业大学软件工程专业本科学历背景，受过多元化教育，拥有较强学习能力和创新精神，习惯了解WEB前端技术领域的最新动态。'
              ]
            },
            {
              type: 1,
              title: '专业水平：',
              text: [
                '专业知识扎实，具备较强独立开发、分析和解决复杂问题的能力。'
              ]
            },
            {
              type: 2,
              title: '专业技能：',
              text: [
                '熟悉HTML/XHTML、CSS等网页制作技术，熟悉页面架构和布局；',
                '对HTML5，CSS3等较新技术也有所了解，能够在开发中使用这些技术；',
                '掌握JavaScript、Ajax等Web开发技术，熟练掌握Bootstrap框架；',
                '对主流前端开库和MVC/MVVM框架(如：Vue.js、Node.js）有较深的理解；',
                '熟悉jQuery，能够使用jQuery完成高效开发，会使用jQuery UI等框架；',
                '熟练使用Chrome，Firebug进行代码调试，具有寻找并修复bug的能力；',
                '对互联网产品和Web技术有浓厚兴趣，有较好的学习能力和强烈的进取心。'
              ]
            },
            {
              type: 1,
              title: '协作能力：',
              text: [
                '较好的执行能力、学习能力，做事认真仔细，注重细节，有责任心，抗压能力较强，拥有良好的团队精神，能与团队一起超额完成工作内容。'
              ]
            },
            {
              type: 1,
              title: '性格爱好：',
              text: [
                '具有较强的求知欲，对技术方面追求严谨，能独立分析和解决问题。日常会与别人探讨技术问题。爱好看书，擅长从已有案例进行知识的学习，从而提高自己的技术水平。面对新领域时，习惯制定切实可行的学习计划，能够高效完成工作。'
              ]
            },
          ]
        },
        {
          text: 'EDUCATION BACKGROUND 教育背景',
          color: '#8fb82c',
          context: [
            {
              type: 3,
              title: '',
              text: [
                '2015.09-2019.06',
                '浙江工业大学',
                '软件工程（工程教育专业认证）'
              ]
            },
            {
              type: 1,
              title: '学校简介：',
              text: [
                '首批省属重点大学，国家“2011计划”首批14所牵头高校。'
              ]
            },
            {
              type: 1,
              title: '主修课程：',
              text: [
                '数据结构、C＋＋程序设计、JAVA程序设计、数据库原理及应用、操作统原理、JavaWeb、软件工程、软件项目管理、算法设计与分析等。'
              ]
            },
            {
              type: 1,
              title: '专业能力：',
              text: [
                '熟练掌握软件工程方面知识和技能，具备从事软件需求分析、软件设计、软件测试、软件维护和软件项目管理等工作的能力。'
              ]
            },
          ]
        },
        {
          text: 'CAMPUS PRACTICE 校园实践',
          color: '#e46e6e',
          context: [
            {
              type: 4,
              title: '',
              text:[
                {time:'2016.09~2018.06',department:'浙江工业大学网络文化工作室',position:'工作室主任'},
                {time:'2017.06~2018.06	',department:'浙江工业大学精弘网络',position:'主席'},
                {time:'2016.06~2017.06	',department:'浙江工业大学精弘网络',position:'主席助理'},
                {time:'2015.09~2016.06',department:'浙江工业大学精弘网络',position:'组织部、开发部部员'}
              ]
            },
            {
              type: 1,
              title: '活动心得：',
              text: [
                '在学校最强的技术型组织中，学到了很多工作技能，掌握了更多专业技能，培养了良好的团队合作精神和高度的责任感。具备较强的团队协作能力、沟通能力、学习能力、抗压能力和创新精神，具备了面对复杂问题的分析和解决能力，养成了积极主动、耐心细致的工作作风。'
              ]
            },
          ]
        },
        {
          text: 'INTERNSHIP EXPERIENCE 实习经历',
          color: '#e46e6e',
          context: [
            {
              type: 1,
              title: '实习单位：',
              text: [
                '杭州银行股份有限公司-软件开发中心-软件开发工程师'
              ]
            },
            {
              type: 1,
              title: '实习时间：',
              text: [
                '2018年7月2日~2018年9月30日'
              ]
            },
            {
              type: 1,
              title: '工作内容：',
              text: [
                '实习过程中参与了两个项目：杭州银行微信网厅和杭州银行手机App的开发。在微信网厅中负责签到领取话费模块前端、弱用户登录后台和前端单元测试、端到端测试、打包分析。在手机银行App项目中负责在线客服页面开发，对接只能客服机器人页面。'
              ]
            },
            {
              type: 1,
              title: '学习技能：',
              text: [
                '在项目开发过程中，学习使用了SVN、STS、FileZilla、VS Code、sublime、SecureCRT、PLSQL Oracle DB等软件，对Vue、JQuery、Java、Linux、Oracle有了更深的理解。'
              ]
            },
          ]
        },
        {
          text: 'GET THE HONOR 获得荣誉',
          color: '#34a6d1',
          context: [
            {
              type: 5,
              title: '',
              text:[
                '2017年7月第七届全国大学生电子商务挑战赛总决赛团队三等奖',
                '2017年5月浙江省“财通证券杯”第十二届大学生电子商务竞赛省赛团队一等奖',
                '学校第十六、十七、十八届办公技能大赛三次分别获得一、二、三等奖各一次',
                '2016、2017年分别获得校级优秀团员、校级优秀团干',
                '2015至2017年主办校第一、第二、第三届网络安全知识竞赛'
              ]
            }
          ]
        }
      ]
    }
  }
}
</script>
