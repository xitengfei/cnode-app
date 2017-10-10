<template>
  <div class="home">
    <md-toolbar>
      <md-button class="md-icon-button" @click="toggleLeftSidenav">
        <md-icon>menu</md-icon>
      </md-button>
      <h2 class="md-title" style="flex: 1">CNode Zone</h2>
    </md-toolbar>
    
    <side-nav ref="sidenav"></side-nav>
    
    <div class="list-view topic-list">
      <ul>
        <li class="item">
          <div class="header"><span>问答</span><h3>对于一个开源的基于Node.js量化交易平台有什么建议?</h3></div>
          <div class="content">
            <div class="userinfo">
              <a href="/"><img src="https://avatars0.githubusercontent.com/u/1655233?v=4&s=120" alt="avatar" /></a>
              <div class="username">似水年华</div>
            </div>
            <div class="metas">
              <p><span class="reply">1</span> / <span class="view">20</span></p>
              <p class="timeago">1小时前</p>
            </div>
          </div>
        </li>
        <li class="item">
          <div class="header"><span>问答</span><h3>对于一个开源的基于Node.js量化交易平台有什么建议?</h3></div>
          <div class="content">
            <div class="userinfo">
              <a href="/"><img src="https://avatars0.githubusercontent.com/u/1655233?v=4&s=120" alt="avatar" /></a>
              <div class="username">似水年华</div>
            </div>
            <div class="metas">
              <p><span class="reply">1</span> / <span class="view">20</span></p>
              <p class="timeago">1小时前</p>
            </div>
          </div>
        </li>
        <li class="item">
          <div class="header"><span>问答</span><h3>对于一个开源的基于Node.js量化交易平台有什么建议?</h3></div>
          <div class="content">
            <div class="userinfo">
              <a href="/"><img src="https://avatars0.githubusercontent.com/u/1655233?v=4&s=120" alt="avatar" /></a>
              <div class="username">似水年华</div>
            </div>
            <div class="metas">
              <p><span class="reply">1</span> / <span class="view">20</span></p>
              <p class="timeago">1小时前</p>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>


<script type="text/javascript">
import SideNav from './SideNav'
export default {
  name: 'home',
  methods: {
    toggleLeftSidenav () {
      this.$refs.sidenav.$refs.leftSidenav.toggle()
    }
  },
  components: {
    SideNav
  }
}
</script>

<style type="text/css">
  .list-view{background:#fff;}
  .list-view li{border-bottom: 1px solid #ddd;padding: 0.2rem;}
  .topic-list{
    .header{display: -webkit-box;display: -ms-flexbox;display: flex;align-items: center;}
  }
  .topic-list .header h3{width:80%;font-size:0.32rem;line-height: 0.56rem;text-overflow: ellipsis;overflow: hidden;white-space: nowrap;}
  .topic-list .header span{font-size:0.24rem;margin-right:0.1rem;padding:0.01rem;background:#2196f3;border-radius:0.06rem;}
</style>