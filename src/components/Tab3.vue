<template>
 <div class="list ticket">
  <form action="###">
    <h2>机票预定</h2>
    <fieldset class="type">
      <p>航程类型 <mark>单程</mark> 往返</p>
    </fieldset>
    <fieldset class="form">
      <p>
        <label for="from_city">出发城市</label>
        <input type="text" name="from_city" id="from_city" placeholder="城市名">
      </p>
      <p>
        <label for="to_city">返回城市</label>
        <input type="text" name="to_city" id="to_city" placeholder="城市名">
      </p>
    </fieldset>
    <fieldset class="form">
      <p>
        <label for="from_date">出发时间</label>
        <input type="text" name="from_date" id="from_date" placeholder="时间/日期">
      </p>
      <p>
        <label for="to_date">返回时间</label>
        <input type="text" name="to_date" id="to_date" placeholder="时间/日期">
      </p>
    </fieldset>
    <fieldset class="form">
      <p>
        <button type="submit" class="submit">订票</button>
      </p>
    </fieldset>
  </form>
  <div class="new">
    <h2>最新机票</h2>
    <ul>
      <li>热门城市：</li>
      <li>北京</li>
      <li>上海</li>
      <li>广州</li>
      <li>深圳</li>
      <li>重庆</li>
      <li>成都</li>
      <li>杭州</li>
      <li>南京</li>
    </ul>
    <table>
      <thead>
        <tr>
          <th>路线</th>
          <th>日期</th>
          <th>价格</th>
          <th class="min">税费</th>
          <th class="min">餐食</th>
          <th>航班</th>
          <th>预定</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>北京-成都</td>
          <td>10-15</td>
          <td class="price">¥745</td>
          <td class="min">¥50</td>
          <td class="min">有</td>
          <td>春秋航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-上海</td>
          <td>10-15</td>
          <td class="price">¥479</td>
          <td class="min">¥45</td>
          <td class="min">无</td>
          <td>南方航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-深圳</td>
          <td>10-15</td>
          <td class="price">¥561</td>
          <td class="min">¥52</td>
          <td class="min">有</td>
          <td>西部航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-杭州</td>
          <td>10-15</td>
          <td class="price">¥378</td>
          <td class="min">¥36</td>
          <td class="min">无</td>
          <td>天津航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-广州</td>
          <td>10-15</td>
          <td class="price">¥612</td>
          <td class="min">¥44</td>
          <td class="min">有</td>
          <td>首都航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-重庆</td>
          <td>10-15</td>
          <td class="price">¥428</td>
          <td class="min">¥62</td>
          <td class="min">有</td>
          <td>东方航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-昆明</td>
          <td>10-15</td>
          <td class="price">¥509</td>
          <td class="min">¥35</td>
          <td class="min">无</td>
          <td>厦门航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-厦门</td>
          <td>10-15</td>
          <td class="price">¥893</td>
          <td class="min">¥73</td>
          <td class="min">有</td>
          <td>深圳航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
        <tr>
          <td>北京-长沙</td>
          <td>10-15</td>
          <td class="price">¥663</td>
          <td class="min">¥46</td>
          <td class="min">无</td>
          <td>四川航空</td>
          <td><a href="###" class="reserve">预定</a></td>
        </tr>
      </tbody>
      <tfoot>
        <tr><td colspan="7"><a href="###" class="more2">加载更多航班...</a></td>
      </tr></tfoot>
    </table>
  </div>
</div>
</template>

<script>
export default {
  data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg: 'Hello World!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>
