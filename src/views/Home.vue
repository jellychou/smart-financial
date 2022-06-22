<template>
  <div>
    <nav class="navbar bg-white fixed-top header_bar" id="app">
      <div class="container-fluid">
        <a class="navbar-brand" href="#" id="top">
            <img src="../assets/image/logo.png" alt="">
        </a>
        <ul class="header_item">
            <li id="tab_1" class="px-3 border-end">為什麼要理財</li>
            <li id="tab_2" class="px-3 border-end">智慧理財靠方法</li>
            <li id="tab_3" class="px-3 border-end">存好股 找元大</li>
            <li id="menu_text" class="px-3 position-relative" @click="toggleMenu">基金申購與管理教學</li>
            <ul class="pc_menu" :class="{ openMenu : isOpen }">
                <li id="tab_4">
                    <img src="../assets/image/1.png" alt="">
                    <div>基金申購</div>
                </li>
                <li id="tab_5">
                    <img src="../assets/image/2.png" alt="">
                    <div>百元投資</div>
                </li>
                <li id="tab_6">
                    <img src="../assets/image/3.png" alt="">
                    <div>基金總覽</div>
                </li>
                <li id="tab_7">
                    <img src="../assets/image/4.png" alt="">
                    <div>基金到價通知</div>
                </li>
                <li id="tab_8">
                    <img src="../assets/image/5.png" alt="">
                    <div>基金損益通知</div>
                </li>
            </ul>
            <img class="header_flower" src="../assets/image/flower.png" alt="">
        </ul>
        <a href="#" class="menu" @click="openMbMenu">
            <img src="../assets/image/menu.png" alt="">
        </a>
        <div class="menu_list" :class={isOpen:isMbOpen}>
            <ul>
                <li class="list_item py-3 py-md-4 text-left">為什麼要理財</li>
                <li class="list_item py-3 py-md-4 text-left">智慧理財靠方法</li>
                <li class="list_item py-3 py-md-4 text-left">存好股 找元大</li>
                <li class="list_item py-3 py-md-4 text-left d-flex align-items-center justify-content-between">
                    <div>基金申購與管理教學</div>
                    <img class="arrow" src="../assets/image/menu_arrow.png" alt="">
                </li>
                <ul class="items">
                    <li class="py-3 item">
                        <img src="../assets/image/1.png" alt="">
                        <div>基金申購</div>
                    </li>
                    <li class="py-3 item">
                        <img src="../assets/image/2.png" alt="">
                        <div>百元投資</div>
                    </li>
                    <li class="py-3 item">
                        <img src="../assets/image/3.png" alt="">
                        <div>基金總覽</div>
                    </li>
                    <li class="py-3 item">
                        <img src="../assets/image/4.png" alt="">
                        <div>基金到價通知</div>
                    </li>
                    <li class="py-3 item">
                        <img src="../assets/image/5.png" alt="">
                        <div>基金損益通知</div>
                    </li>
                </ul>
            </ul>
        </div>
        <img class="header_plus" src="../assets/image/header-plus.png" alt="">
      </div>
    </nav>
    <div class="banner">
        <img class="scene" src="../assets/image/top_back.png" alt="">
        <img class="scene" src="../assets/image/top_medium.png" alt="">
        <img class="scene" src="../assets/image/top_front.png" alt="">
        <div class="sidebar_1">
          <img src="../assets/image/sidebar1.png" alt="">
          <div class="sidebar_text">信託開戶</div>
        </div>
        <div class="sidebar_2">
          <img src="../assets/image/sidebar2.png" alt="">
          <div class="sidebar_text">線上開戶</div>
        </div>
    </div>
    <div class="banner_mb">
        <img class="scene" src="../assets/image/back.png" alt="">
        <img class="scene" src="../assets/image/medium.png" alt="">
        <img class="scene" src="../assets/image/front.png" alt="">
    </div>
    <div class="position-relative">
        <img class="second_cloud" src="../assets/image/lightblue@3x.png" alt="">
    </div>
    <div class="bg_light">
        <div class="container-xl">
            <div class="step_1" id="step_1">
                <div class="step_1_title">為什麼要理財？</div>
                <div class="step_1_content">
                    <span class="quota_left">“</span>
                    一輩子能夠累積多少財富，不取決於你能夠賺多少錢，而取決於你如何投資理財。
                    <span class="quota_right">”</span>
                </div>
                <hr class="dash_line" />
                <div class="step_1_by">股神 巴菲特</div>
            </div>
            <div class="d-sm-flex align-items-center justify-content-around">
                <img class="sec_1" src="../assets/image/sec1.png" alt="">
                <div class="save_sec">
                    <div class="save_text mb-3">通膨壓力上升，小心你的錢越存越薄！</div>
                    <div class="save_text">越早開始理財，就能避免通膨吃掉你的錢，還能越早存</div>
                    <div class="save_text">到理想生活的第一桶金，提升生活品質，豐富人生！</div>
                </div>
            </div>
            <div class="step_2">
                新手理財 Tips
                <img class="shine" src="../assets/image/shine.png" alt="">
            </div>
            <ul class="d-sm-flex align-items-center justify-content-around">
                <li class="tips_card">
                    <img src="../assets/image/icon1.png" alt="">
                    <div class="tips_title">神奇的複利效應</div>
                    <div class="tips_content">及早開始，紀律投資，投資效益就會如滾雪球一樣越滾越大</div>
                </li>
                <li class="tips_card">
                    <img src="../assets/image/icon2.png" alt="">
                    <div class="tips_title">專注於長期趨勢</div>
                    <div class="tips_content">定期投入，降低平均成本，讓資產跟著市場一起成長</div>
                </li>
                <li class="tips_card">
                    <img src="../assets/image/icon3.png" alt="">
                    <div class="tips_title">小額輕鬆開始</div>
                    <div class="tips_content">小資金也能投資，基金、ETF 理財無負擔</div>
                </li>
            </ul>
            <div class="step_3">
                如何邁出理財第一步？
                <img class="shine" src="../assets/image/shine.png" alt="">
            </div>
            <ul class="d-sm-flex align-items-center justify-content-around">
                <li class="tab_card">
                    <div class="step_tab">基金</div>
                    <div>
                        <div class="d-flex align-items-start mb-2">
                            <img class="pt-2" src="../assets/image/listdot.png" alt="">
                            <div class="step_list">少少資金投資多元標的，單筆投入也能分散風險</div>
                        </div>
                        <div class="d-flex align-items-start">
                            <img class="pt-2" src="../assets/image/listdot.png" alt="">
                            <div class="step_list">讓專業經理人幫你管理投資組合，節省研究時間</div>
                        </div>
                    </div>
                </li>
                <li class="tab_card">
                    <div class="step_tab">ETF</div>
                    <div>
                        <div class="d-flex align-items-start mb-2">
                            <img class="pt-2" src="../assets/image/listdot.png" alt="">
                            <div class="step_list">投資管道多元，方便有彈性；交易成本低，小資無負擔</div>
                        </div>
                        <div class="d-flex align-items-start">
                            <img class="pt-2" src="../assets/image/listdot.png" alt="">
                            <div class="step_list">產品選擇豐富，各市場、產業及商品都有相應標的可投資</div>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
        <img class="flowers" src="../assets/image/flowers.png" alt="">
        <img class="darkblue" src="../assets/image/darkblue.png" alt="">
    </div>
    <div class="bg-darkBlue">
        <div class="container-xl">
            <div class="step_4" id="step_4">
                <div class="financial_method_title">智慧理財靠方法</div>
                <div class="financial_method_subtitle">元大日日扣  定期定額百元投資法</div>
                <ul class="d-sm-flex align-items-center justify-content-around">
                    <li>
                        <img class="pig" src="../assets/image/pig.png" alt="">
                    </li>
                    <li>
                        <div class="invest_title">每天都是投資天</div>
                        <div class="invest_text">定期定額日日扣創造投資機會點。</div>
                        <div class="invest_text">長期紀律投資，讓定期定額微笑曲線更快發生。</div>
                        <div class="invest_button">前往了解 ></div>
                    </li>
                </ul>
                <ul class="d-sm-flex align-items-center justify-content-around py-5">
                    <li class="d-flex align-items-center feature_card">
                        <img src="../assets/image/feature1.png" alt="">
                        <div class="feature">
                            <div class="feature_log">Feature 1</div>
                            <div class="feature_title">彈性選擇</div>
                            <div class="feature_content">打破傳統每月扣款次數、日期、金額限制，視個人理財計畫需求，例如每隔 1 天、7 天或 10 天自由挑選每月扣款日。</div>
                        </div>
                    </li>
                    <li class="d-flex align-items-center feature_card">
                        <img src="../assets/image/feature2.png" alt="">
                        <div class="feature">
                            <div class="feature_log">Feature 1</div>
                            <div class="feature_title">分散風險</div>
                            <div class="feature_content">市場波動時，透過更頻繁的扣款次數或調整扣款金額，例如分拆為多次較小額資金，有助於進一步分散進場時間點的風險。</div>
                        </div>
                    </li>
                </ul>
                <div class="step_calculation">
                    <div class="d-flex align-items-center justify-content-between calculation px-md-5 px-2">
                        <div>立即進行定期定額試算</div>
                        <img src="../assets/image/count.png" alt="">
                    </div>
                    <div class="calculation_card">
                        <div class="card_title">輸入您的投資試算條件，模擬未來投資結果！</div>
                        <div class="tab_list mx-2 mx-md-2 mx-lg-5 range-slider" >
                            <div class="d-flex align-items-center justify-content-between py-md-3">
                                <div class="items_title">每月投資金額</div>
                                <div>
                                    <input @input="inputSlider(1)" type="number" required="" class="range-slider__value f24 input_style" v-model="sliderValue_1" max="20000" name="amount">
                                    <span class="unit">元</span>
                                </div>
                            </div>
                            <input @change="changeSlider(1)" class="range-slider__range" type="range" v-model="value_1" min="0" max="20000" step="1000" :style="getSliderBlue_1">
                            <div class="number_bar d-flex align-items-center justify-content-between py-md-3">
                                <div>0 <span>元</span> </div>
                                <div>20,000 <span>元</span> </div>
                            </div>
                        </div>
                        <div class="tab_list mx-2 mx-md-2 mx-lg-5 range-slider">
                            <div class="d-flex align-items-center justify-content-between py-md-3">
                                <div class="items_title">目標投資年報酬率<span>（ 僅能輸入 5-12 之數值 ）</span></div>
                                <div>
                                    <input  @input="inputSlider(2)" type="number" required="" class="range-slider__value f24 input_style" v-model="sliderValue_2" max="20000" name="amount">
                                    <span class="unit">％</span>
                                </div>
                            </div>
                            <input @change="changeSlider(2)" class="range-slider__range" type="range" v-model="value_2" min="5" max="12" step="1" :style="getSliderBlue_2">
                            <div class="number_bar d-flex align-items-center justify-content-between py-md-3">
                                <div>5 <span>％</span> </div>
                                <div>12 <span>％</span> </div>
                            </div>
                        </div>
                        <div class="tab_list mx-2 mx-md-2 mx-lg-5">
                            <div class="d-flex align-items-center justify-content-between py-md-3">
                                <div class="items_title">投資期間</div>
                                <div>
                                    <input @input="inputSlider(3)" type="number" required="" class="range-slider__value f24 input_style" v-model="sliderValue_3" max="20000" name="amount">
                                    <span class="unit">年</span>
                                </div>
                            </div>
                            <input @change="changeSlider(3)" class="range-slider__range" type="range" v-model="value_3" min="0" max="40" :style="getSliderBlue_3">
                            <div class="number_bar d-flex align-items-center justify-content-between py-md-3">
                                <div>0 <span>年</span> </div>
                                <div>40 <span>年</span> </div>
                            </div>
                        </div>
                        <ul class="calculation_total mx-1 mx-md-2 mx-lg-5 my-4 d-sm-flex align-items-center justify-content-around">
                            <li class="total_card">
                                <div class="total_title">投資到期總金額</div>
                                <div class="d-flex justify-content-center pt-3">
                                    <div class="dashed_dollar"></div>
                                    <span class="total_unit">元</span>
                                </div>
                            </li>
                            <li class="total_card">
                                <div class="total_title">投資到期總金額</div>
                                <div class="d-flex justify-content-center pt-3">
                                    <div class="dashed_dollar"></div>
                                    <span class="total_unit">元</span>
                                </div>
                            </li>
                            <li class="total_card">
                                <div class="total_title">投資到期總金額</div>
                                <div class="d-flex justify-content-center pt-3">
                                    <div class="dashed_dollar"></div>
                                    <span class="total_unit">元</span>
                                </div>
                            </li>
                        </ul>
                        <div class="illustrate mx-4 mx-md-2 mx-lg-5">說明：此區是以IRR報酬率試算的結果，僅供投資人理財參考。該數字未考量物價通貨膨脹率及風險係數，且未加計任何可能產生的手續費用和稅金，也無保證和實際投資狀況相符。投資人因不同時間進場，將有不同之投資績效，過去之績效亦不代表未來績效之保證，資料模擬之結果僅供參考，不代表實際報酬率及未來績效保證，不同時間進行模擬試算，其結果亦可能不同。註: IRR (Internal Rate of Return)中文可翻譯為內部報酬率，簡單來說就是將報酬率加入時間成本跟現金流的概念，是一種投資的評估方法。</div>
                    </div>
                </div>
            </div>
        </div>
        <img class="flowers" src="../assets/image/flowers.png" alt="">
        <img class="darkblue" src="../assets/image/lightblue.png" alt="">
    </div>
    <div class="bg_light">
        <div class="container-xl">
            <div class="step_5" id="step_5">
                <div class="save_title">存好股 找元大</div>
                <div class="discount_text">
                    <img src="../assets/image/shine_blue.png" alt="">
                    限時優惠中
                    <img src="../assets/image/shine_blue.png" alt="">
                </div>
                <div class="discount_time">（即日起至 <span>2022/9/30</span> ）</div>
            </div>
            <ul class="d-sm-flex align-items-center justify-content-around">
                <li class="save">
                    <div class="save_tab">基金</div>
                    <div class="save_tab_title">線上申購指定基金，定期（不）定額</div>
                    <div class="save_slogan">
                        <img src="../assets/image/oringin_shine.png" alt="">
                        享終身優惠  <span>0</span> 手續費
                        <img src="../assets/image/oringin_shine.png" alt="">
                    </div>
                    <div class="save_tab_subtitle">指定基金</div>
                    <div class="save_tab_content">
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大卓越基金</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大多福基金</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大經貿基金</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大高科技基金</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大 2001 基金</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大台灣高股息優質龍頭基金（<span>本基金之配息來源可能為收益平準金</span>）</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                    </div>
                </li>
                <li class="save">
                    <div class="save_tab">ETF</div>
                    <div class="save_tab_title">線上申購指定國內 ETF，定期（不）定額</div>
                    <div class="save_slogan">
                        <img src="../assets/image/oringin_shine.png" alt="">
                        享終身手續費<span>0.3%</span>
                        <img src="../assets/image/oringin_shine.png" alt="">
                    </div>
                    <div class="save_tab_subtitle">指定國內 ETF</div>
                    <div class="save_tab_content">
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大台灣卓越50基金 (0050ETF)</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大台灣高股息基金 (0056ETF)</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大臺灣ESG永續ETF (00850)</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="save_list d-flex align-items-center justify-content-between py-3 py-md-1">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">元大全球未來通訊ETF (00861)</div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="d-flex align-items-center justify-content-between pt-3">
                            <div class="d-flex align-items-center">
                                <img src="../assets/image/listdot.png" alt="">
                                <div class="save_list_title">
                                    元大全球5G關鍵科技ETF基金 (00876)
                                </div>
                            </div>
                            <img class="link_icon" src="../assets/image/link.png" alt="">
                            <img class="link_active" src="../assets/image/link_active.png" alt="">
                        </div>
                        <div class="remark">(原:元大全球未來關鍵科技ETF基金)</div>
                        <div class="empty_parameter"></div>
                    </div>
                </li>
            </ul>
        </div>
        <img class="flowers" src="../assets/image/flowers.png" alt="">
        <img class="darkblue" src="../assets/image/darkblue.png" alt="">
    </div>
    <div class="bg-darkBlue position-relative">
        <div class="container-xl">
           <div class="step_6">洞悉基金動態 元大行動銀行好幫手</div>
           <ul id="tab" class="tab d-flex align-items-center justify-content-center">
                <li :class="tabItem === 1 ? 'active_tab' : 'normal_tab'" @click="fetchTab(1)"><div>基金申購</div></li>
                <li :class="tabItem === 2 ? 'active_tab' : 'normal_tab'" @click="fetchTab(2)"><div>百元投資</div></li>
                <li :class="tabItem === 3 ? 'active_tab' : 'normal_tab'" @click="fetchTab(3)"><div>基金總覽</div></li>
                <li :class="tabItem === 4 ? 'active_tab' : 'normal_tab'" @click="fetchTab(4)"><div>基金到價通知</div></li>
                <li :class="tabItem === 5 ? 'active_tab' : 'normal_tab'" @click="fetchTab(5)"><div>基金損益通知</div></li>
           </ul>
           <div class="single_subscription">
                <div class="single_title">基金單筆申購流程教學</div>
                <div class="single_subtitle">簡單幾步驟 快速完成基金單筆申購</div>
                <ul v-if="stepNumber === 4" class="number_step d-flex align-items-center justify-content-between four_step">
                    <li @click="goStep" :style="{'--bgImage': bgLine_4}" :class="getActiveNumber(item)" v-for="item in 4" :key="item">0{{ item }}</li>
                </ul>
                <ul v-if="stepNumber === 5" class="number_step d-flex align-items-center justify-content-between five_step">
                    <li @click="goStep" :style="{'--bgImage': bgLine_5}" :class="getActiveNumber(item)" v-for="item in 5" :key="item">0{{ item }}</li>
                </ul>
                <ul v-if="stepNumber === 6" class="number_step d-flex align-items-center justify-content-between six_step">
                    <li @click="goStep" :style="{'--bgImage': bgLine_6}" :class="getActiveNumber(item)" v-for="item in 6" :key="item">0{{ item }}</li>
                </ul>
                <div v-if="stepNumber === 9">
                  <ul class="number_step d-flex align-items-center justify-content-between nine_step">
                      <li @click="goStep" :style="{'--bgImage': bgLine_9}" :class="getActiveNumber(1)" :key="item">01</li>
                      <li @click="goStep" :style="{'--bgImage': bgLine_9}" :class="getActiveNumber(2)" :key="item">02</li>
                      <li @click="goStep" :style="{'--bgImage': bgLine_9}" :class="getActiveNumber(3)" :key="item">03</li>
                      <li @click="goStep" :style="{'--bgImage': bgLine_9}" :class="getActiveNumber(4)" :key="item">04</li>
                      <li @click="goStep" :style="{'--bgImage': bgLine_9}" :class="getActiveNumber(5)" :key="item">05</li>
                      <li @click="goStep" :style="{'--bgImage': bgLine_9}" :class="getActiveNumber(6)" :key="item">06</li>
                  </ul>
                  <ul class="number_step d-flex align-items-center justify-content-between nine_2_step">
                      <li @click="goStep" :style="{'--bgImage': bgLine_10}" :class="getActiveNumber(7)" :key="item">07</li>
                      <li @click="goStep" :style="{'--bgImage': bgLine_10}" :class="getActiveNumber(8)" :key="item">08</li>
                      <li @click="goStep" :style="{'--bgImage': bgLine_10}" :class="getActiveNumber(9)" :key="item">09</li>
                  </ul>
                </div>
                <div class="d-sm-flex align-items-center justify-content-center my-5">
                    <img @click="preImage" class="pre_icon" src="../assets/image/previous.png" alt="">
                    <div class="phone">
                        <img id="phone" class="phone_body" :src="thisImage" alt="">
                        <img class="phone_out" src="../assets/image/phone.png" alt="">
                    </div>
                    <div class="bubble">
                        <img class="bubble_mb" src="../assets/image/bubble_mb.png" alt="">
                        <img class="bubble_pc" src="../assets/image/bubble.png" alt="">
                        <div id="bubble_title" class="bubble_title">STEP{{ step }}</div>
                        <div id="bubble_content" class="bubble_content">{{ content }}</div>
                        <div class="step_button">前往了解 ></div>
                    </div>
                    <img @click="nextImage" class="next_icon" src="../assets/image/next.png" alt="">
                </div>
           </div>
        </div>
        <!--<img class="web" src="./image/web.png" alt="">-->
        <img class="flowers" src="../assets/image/flowers.png" alt="">
        <img class="darkblue" src="../assets/image/white.png" alt="">
    </div>
    <div class="bg_white">
        <div class="container-xl">
            <div class="third">
                <div class="third_title">立即加入官方社群 隨時掌握元大銀行最新消息</div>
                <div class="d-flex align-items-center justify-content-center">
                    <div class="row third_step d-flex align-items-center justify-content-around">
                        <div class="col-6 col-md-4 col-lg-2 third_icon" @click="newPage('fans')">
                            <div class="third_circle">
                                <img src="../assets/image/fb.png" alt="">
                            </div>
                            <div class="third_text pt-3">元大銀行鑽金生活</div>
                            <div class="third_text">Fans官方粉絲團</div>
                        </div>
                        <div class="col-6 col-md-4 col-lg-2 third_icon" @click="newPage('line')">
                            <div class="third_circle">
                                <img src="../assets/image/line.png" alt="">
                            </div>
                            <div class="third_text pt-3">元大銀行LINE@</div>
                            <div class="third_text">官方帳號</div>
                        </div>
                        <div class="col-6 col-md-4 col-lg-2 third_icon" @click="newPage('ig')">
                            <div class="third_circle">
                                <img src="../assets/image/ig.png" alt="">
                            </div>
                            <div class="third_text pt-3">元大銀行Instagram</div>
                            <div class="third_text">官方帳號</div>
                        </div>
                        <div class="col-6 col-md-4 col-lg-2 third_icon" @click="newPage('yt')">
                            <div class="third_circle">
                                <img src="../assets/image/yt.png" alt="">
                            </div>
                            <div class="third_text pt-3">元大銀行YouTube</div>
                            <div class="third_text">官方帳號</div>
                        </div>
                        <div class="col-6 col-md-4 col-lg-2 third_icon" @click="newPage('tg')">
                            <div class="third_circle">
                                <img src="../assets/image/tg.png" alt="">
                            </div>
                            <div class="third_text pt-3">元大銀行Telegram</div>
                            <div class="third_text">官方帳號</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <img class="flowers" src="../assets/image/flowers.png" alt="">
        <img class="second_cloud" src="../assets/image/lightblue@3x.png" alt="">
    </div>
    <div class="bg_light">
        <div class="container-xl">
            <div class="notice">
                <div class="notice_title">注意事項</div>
                <div class="notice_content">
                    <div class="notice_content_title">（一）活動規則</div>
                    <ol>
                        <li>活動期間（即日起至 2022 年 09 月 30日）內，客戶透過元大商業銀行股份有限公司（以下簡稱本行）個人網路銀行或行動銀行新增定期(不)定額之元大台灣高股息優質龍頭基金(本基金之配息來源可能為收益平準金)、元大多福基金、元大卓越基金、元大高科技基金、元大經貿基金或元大2001基金定期(不)定額申購扣款設定並成功扣款，即可享該基金定期(不)定額終身優惠0手續費。</li>
                        <li>活動期間（即日起至 2022 年 09 月 30日）內，客戶透過元大商業銀行股份有限公司（以下簡稱本行）個人網路銀行或行動銀行新增定期(不)定額之元大台灣卓越50基金(0050ETF)、元大台灣高股息基金(0056ETF)、元大臺灣ESG永續ETF基金(00850)或元大全球未來通訊ETF基金(00861)、元大全球5G關鍵科技ETF(00876)(原:元大全球未來關鍵科技ETF基金)國內ETF定期(不)定額申購扣款設定並成功扣款，即可享該ETF定期(不)定額終身手續費0.3%。</li>
                    </ol>
                    <div class="notice_content_title">（二）本網站的立場及聲明</div>
                    <ol>
                        <li>本活動係本行舉辦。參加者於參加本活動時，即同意接受本活動規則內容、個人網路銀行、行動銀行APP及元大e櫃檯各項使用規範及規定；如有以不當程式或方法干擾，本行將取消參加本活動及享有手續費優惠之資格，本行並得向參加者請求損害賠償。</li>
                        <li>參加者應承諾提出之資料應均為真實、正確且未冒用或盜用任何第三人之資料；若有冒用或盜用他人資料，或個人資料有不實、不齊全或不正確之情事，本行將取消參加或（及）享有手續費優惠之資格。如因此造成第三人向本行主張任何權利，應由參加者負全部責任。</li>
                        <li>任何因行動裝置、電腦、網路、電話、技術或不可歸責於本行之事由，而使參加者所登錄之資料有遲延、遺失、錯誤、無法辨識或毀損等情況，本行不負任何責任，參加者亦不得因此異議或請求賠償。</li>
                    </ol>
                    <div class="notice_content_title">（三）法律管轄權</div>
                    <ol>
                        <li>參加者同意與本活動有關之任何行為，應依據中華民國法律解釋或辦理，即使使用本行個人網路銀行或行動銀行 APP 之當時所在地非中華民國境內，仍以中華民國法律規範之。</li>
                        <li>雙方同意如因本活動發生相關訴訟，除法律另有規定外，以臺灣臺北地方法院為第一審管轄法院。</li>
                    </ol>
                    <div class="notice_content_title">（四）免責聲明</div>
                    <ol>
                        <li>本行保有審核參加者資格之權利，及取消、終止、修改或暫停本活動規則的權利。</li>
                        <li>如有其他未盡事宜，悉依本行官方網站公告之相關規定或決定辦理。如有疑問，請洽本行客服中心 (02)2182-1968 或 0800-668-168。</li>
                    </ol>
                    <div class="notice_content_title">（五）基金警語 投資一定有風險，基金投資有賺有賠，申購前請詳閱公開說明書 !</div>
                    <ol>
                        <li>【元大投信獨立經營管理】元大系列基金經金管會核准或申報生效，惟不表示絕無風險。元大投信以往之經理績效，不保證基金之最低投資收益；元大投信除盡善良管理人之注意義務外，不負責基金之盈虧，亦不保證最低之收益，投資人因不同時間進場，將有不同之投資績效，過去之績效亦不代表未來績效之保證。投資人申購前應詳閱基金公開說明書。本文提及之經濟走勢預測不必然代表基金之績效，基金投資風險請詳閱基金公開說明書。有關基金運用限制及投資風險、配息機制、基金申購手續費之收取方式，比率、投資人所需負責之直接或間接相關費用及基金應負擔之相關費用，已揭露於基金公開說明書中，投資人可向元大投信及基金之銷售機構索取，或至公開資訊觀測站及元大投信網站（https://www.yuantafunds.com）中查詢。為避免因受益人短線交易頻繁，造成基金管理及交易成本增加，進而損及基金長期持有之受益人權益，元大系列基金不歡迎受益人進行短線交易。基金非存款或保險，故無受存款保險、保險安定基金或其他相關保障機制之保障。元大系列基金之配息率不代表基金報酬率，且過去配息率不代表未來配息率，基金淨值可能因市場因素而上下波動。</li>
                        <li>【元大台灣高股息優質龍頭基金(本基金之配息來源可能為收益平準金)】基金配息可能由基金的收益平準金中支付。任何涉及由收益平準金支出的部分可能導致原始投資金額減損。收益平準金係指本基金成立日起，計算日之每日受益權單位淨資產價值中，相當於原受益人可分配之收益金額。本基金持股之股利配發時間及金額視各別企業而定。主要來自於「高股息優質龍頭」企業發放的現金股利於累積一段期間後，分為12個月，每月分配給投資人。另每月之收益分配係以本基金B 類型受益權單位投資於中華民國境內所得之現金股利、利息收入、已實現股票股利、子基金收益分配及收益平準金等收入扣除應負擔之費用後之可分配收益且不需扣除已實現及未實現之資本損失。每年度分配收益係以本基金B 類型受益權單位投資於中華民國境內所得之已實現資本利得扣除資本損失（包括已實現及未實現之資本損失），並扣除應負擔之費用後之可分配收益。經理公司認為有必要（如市況變化足以對相關基金造成影響）可適時調整收益分配金額，惟本基金B 類型受益權單位可分配收益，於經理公司決定收益分配金額後，若有未分配收益得累積併入以後之可分配收益。B 類型受益權單位之任一受益人應得之分配金額為新臺幣伍佰元（含）以下者，受益人（除基金銷售機構以自己名義受託申購基金專戶、特定金錢信託專戶、財富管理專戶或壽險公司透過投資型保單等方式為投資人申購本基金者外）同意授權經理公司得以該收益分配金額再申購本基金B 類型受益權單位作為當期收益分配之給付方式，該等收益分配金額再申購本基金之申購手續費為零元。
                            基金注意事項：
                        </li>
                            <div>(1)銀行辦理信託業務，應盡善良管理人之注意義務及忠實義務。
                            <div>(2)銀行不擔保信託業務之管理或運用績效，委託人及受益人應自負盈虧。</div>
                            <div>(3)信託財產經運用於存款以外之標的者，不受存款保險之保障，投資人申購前應仔細閱讀行銷文件。</div>
                            <div>(4)基金並非存款，基金投資具有投資風險，可能使本金發生虧損。</div>
                            <div>(5)投資人因不同時間進場，將有不同之投資績效，過去之績效亦不代表未來績效之保證。</div>
                            <div>(6)如基金投資以外幣計價之有價證券，其淨值可能因匯率而變動。</div>
                            <div>(7)現階段法令規定境外基金投資大陸地區證券市場之有價證券以掛牌上市有價證券及銀行間債券市場為限，且投資總金額不得超過該基金淨資產價值20%(境外基金機構依鼓勵境外基金深耕計畫向金管會申請並經認可，得放寬投資總金額上限至40%)，故並非完全投資於大陸地區之有價證券；投信基金投資大陸地區之有價證券雖可包括其證券集中交易市場交易之股票、存託憑證或符合一定信用評等之債券等且法令並無規範投資總金額之上限，惟仍應符合信託契約、公開說明書、證券投資信託基金管理辦法等相關規定及受到基金公司QFII額度之限制，故亦非一定完全投資於大陸地區有價證券。又投資人亦須留意中國市場政府政策、法令、會計稅務制度、經濟與市場等變動所可能產生之投資風險。</div>
                            <div>(8)中國境內債券之信用評級，由中國評級機構所授予，其所使用評級標準與方法可能與其他國際評級機構所採用者不一致，故該評級制度未必可提供同等的標準與獲得國際評級的證券進行比較。</div>
                            <div>(9)由於新興市場基金主要投資風險，除包含一般股票型基金之投資組合跌價與匯率風險外，與成熟市場相比，須承受較高之政治與金融管理風險，且因市值及制度性因素，流動性風險也相對較高，故新興市場投資組合波動性普遍高於成熟市場。</div>
                            <div>(10)投資新興市場可能比投資已開發國家有較大的價格波動及流動性較低的風險。部分基金可能持有衍生性商品部位，可能達基金淨資產價值之100%，可能造成基金淨值高度波動及衍生其他風險，委託人應慎選投資標的。</div>
                            <div>(11)基金配息率不代表基金報酬率，且過去配息率不代表未來配息率；基金淨值可能因市場因素而上下波動。基金的配息可能由基金的收益或本金中支付。任何涉及由本金支出的部分，可能導致原始投資金額減損。基金之配息來源可能為本金。</div>
                            <div>(12)非投資等級債券基金(本類基金主要係投資於非投資等級之高風險債券且配息來源可能為本金)(主要特色係投資前揭基金之組合基金亦同)，適合能承受較高風險之『非保守型』委託人且不宜占投資組合過高的比重。由於非投資等級債券之信用評等未達投資等級或未經信用評等，且對利率變動的敏感度甚高，可能會因利率上升、市場流動性下降，或債券發行機構違約不支付本金、利息或破產而蒙受虧損，不適合無法承擔相關風險之投資人；又如係本國投信機構募集者，則可能投資於符合美國Rule 144A規定具有私募性質之債券，雖其投資總金額不得超過基金淨資產價值之百分之三十，然該債券具有債券發行人違約之信用風險、利率風險、流動性風險、交易對手風險及因財務訊息揭露不完整或因價格不透明導致波動性較大之風險。</div>
                            <div>(13)本專案活動之基金經金管會核准或同意生效，惟不表示絕無風險。基金經理公司以往之經理績效不保證基金之最低投資收益；基金經理公司除盡善良管理人之注意義務外，不負責基金之盈虧，亦不保證最低之收益，投資人申購前應詳閱基金簡式公開說明書及基金公開說明書。</div>
                            <div>(14)委託人之交易如經基金公司認定為短線交易者，基金公司或本行可拒絕受理申請轉換或申購要求，並可請求支付一定比例之贖回費用或其他相關費用，費用標準均依各該基金公司之規定。</div>
                            <div>(15)後收型基金在贖回時，基金公司將依持有期間長短收取不同比率之遞延申購手續費，該費用將自贖回總額中扣除；另各基金公司需收取一定比率之分銷費用，將反映於每日基金淨值中，投資人無需額外支付。</div>
                            <div>(16)有關投資基金應承擔之相關風險(如國家風險、市場風險、貨幣風險、匯率風險、信用風險、債券風險等)及負擔之費用(含分銷費用)，已揭露於基金之公開說明書或投資人須知中，投資人欲索閱基金公開說明書(或其中譯本)或投資人須知，可至本行各分行洽詢理財專員或洽該基金公司，或至公開資訊觀測站或境外基金資訊觀測站(https://www.fundclear.com.tw)查詢。</div></div>
                    </ol>
                    <div class="notice_content_title">（六）國內ETF投資警語：</div>
                    <ol>
                        <li>市場風險：ETF的價格會因經濟、政治、貨幣、法律等各種影響市場因素而波動。</li>
                        <li>集中度風險：ETF通常分散持有一籃子投資組合，較不受個別標的風險影響，然而，有些ETF仍可能有曝險集中於少數個股、集中投資於特定產業或單一商品的情形。</li>
                        <li>流動性風險：ETF流動量提供者負責提供ETF買賣報價，方便投資人買賣ETF。儘管ETF大部分有一個或以上的流動量提供者，但若有流動量提供者失責或停止履行報價義務，投資人可能會有買不到或是賣不掉ETF的風險。</li>
                        <li>折溢價風險：ETF市價由市場供需決定，可能低於或高於淨值而產生折價或溢價。折溢價過大代表ETF成交價格產生偏離。此外，連結海外標的之ETF可能因國內外市場交易時間差而有折溢價情形。</li>
                        <li>追蹤誤差風險：追蹤誤差係指ETF報酬率與標的指數報酬率的差異程度。產生追蹤誤差的原因很多，包括基金須支付的費用及支出影響、基金資產與指數成分股之差異、基金的計價貨幣、交易貨幣及投資所用的貨幣間的匯率差價，ETF投資組合的成分股配股配息、基金經理人所使用的追蹤工具及複製策略等，皆會造成ETF的資產淨值與股價指數間存在落差。</li>
                        <li>終止上市風險：發行人可能因ETF資產規模太小、單位淨值過低等信託契約規定的終止情事，報請主管機關核准終止信託契約並申請下市。</li>
                    </ol>
                </div>
                <div class="footer_address">
                    <div>【元大銀行總址地址：臺北市松山區敦化南路一段66號；聯絡電話：(02)2173-6699】</div>
                    <div>詳情歡迎親洽本行各分行理財業務專員，或撥0800-688-168，或至本行網站：www.yuantabank.com.tw查詢。</div>
                </div>
            </div>
        </div>
        <div class="footer">
            <div class="pb-2">Copyright © Yuanta Commercial Bank Co. Ltd. All Rights Reserved.</div>
            <div>地址：10557 台北市松山區敦化南路一段 66 號 ｜ 電子信箱：Service@yuanta.com ｜ 客服專線：0800-688-168</div>
        </div>
        <ul class="open_account">
          <li>
            <div class="open_account_card d-flex align-items-center justify-content-center">
                <img src="../assets/image/sidebar1.png" alt="">
                <div class="account_text">信託開戶</div>
            </div>
          </li>
          <li>
             <div class="open_account_card d-flex align-items-center justify-content-center">
              <img src="../assets/image/sidebar2.png" alt="">
              <div class="account_text">線上開戶</div>
            </div>
          </li>
        </ul>
    </div>
    <div class="to_top">
        <img src="../assets/image/top.png" alt="" @click="goTop">
        <div>TOP</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      step: 0,
      tabItem: 1,
      thisImage: '',
      stepNumber: 0,
      content: '',
      isOpen: false,
      isMbOpen: false,
      sliderValue_1: 0,
      sliderValue_2: 5,
      sliderValue_3: 0,
      blue_1: 0,
      blue_2: 0,
      blue_3: 0,
      value_1: 0,
      value_2: 0,
      value_3: 0,
      startCounter: '',
      bgLine_4: 0,
      bgLine_5: 0,
      bgLine_6: 0,
      bgLine_9: 0,
      phoneImage: [
        {
          step: [
            {
              id: 1,
              content: '行動銀行首頁點基金單筆申購',
              img: require('../assets/image/1-1.png')
            },
            {
              id: 2,
              content: '選擇欲申購基金之資料並看完下方說明後打勾',
              img: require('../assets/image/1-2.png')
            },
            {
              id: 3,
              content: '閱讀並確認基金申購相關文件',
              img: require('../assets/image/1-3.png')
            },
            {
              id: 4,
              content: '確認交易資訊並輸入交易密碼',
              img: require('../assets/image/1-4.png')
            },
            {
              id: 5,
              content: '交易成功',
              img: require('../assets/image/1-5.png')
            }
          ]
        },
        {
          step: [
            {
              id: 1,
              content: '行動銀行首頁點基金總覽',
              img: require('../assets/image/2-3.png')
            },
            {
              id: 2,
              content: '點選百元投資',
              img: require('../assets/image/2-3.png')
            },
            {
              id: 3,
              content: '選擇欲申購基金之資料且設定每月扣款日期，並看完下方說明後打勾',
              img: require('../assets/image/2-3.png')
            },
            {
              id: 4,
              content: '閱讀並確認基金申購相關文件',
              img: require('../assets/image/2-4.png')
            },
            {
              id: 5,
              content: '確認交易資訊並輸入交易密碼',
              img: require('../assets/image/2-5.png')
            },
            {
              id: 6,
              content: '交易成功',
              img: require('../assets/image/2-6.png')
            }
          ]
        },
        {
          step: [
            {
              id: 1,
              content: '行動銀行首頁點基金總覽',
              img: require('../assets/image/3-2.png')
            },
            {
              id: 2,
              content: '進入基金總覽頁可察看各庫存標的之績效 1.可以查詢基金交易明細 2.預覽庫存資訊（顯示五檔並以市值由高至低排序）',
              img: require('../assets/image/3-2.png')
            },
            {
              id: 3,
              content: '切換申購清單，可以瀏覽各種投資方式及其庫存標的現況',
              img: require('../assets/image/3-3.png')
            },
            {
              id: 4,
              content: '點擊該庫存標的後可以查看更詳細資訊 (ex.手續費、配息…等)',
              img: require('../assets/image/3-4.png')
            }
          ]
        },
        {
          step: [
            {
              id: 1,
              content: '行動銀行首頁點選設定',
              img: require('../assets/image/4-2.png')
            },
            {
              id: 2,
              content: '點選基金到價通知設定',
              img: require('../assets/image/4-2.png')
            },
            {
              id: 3,
              content: '點選新增',
              img: require('../assets/image/4-3.png')
            },
            {
              id: 4,
              content: '設定欲通知標的/淨值上下限/通知起訖日',
              img: require('../assets/image/4-4.png')
            },
            {
              id: 5,
              content: '標的通知設定成功',
              img: require('../assets/image/4-5.png')
            },
            {
              id: 6,
              content: '回行動銀行首頁點選設定，繼續設定系統通知',
              img: require('../assets/image/4-6.png')
            },
            {
              id: 7,
              content: '點選訊息通知設定',
              img: require('../assets/image/4-7.png')
            },
            {
              id: 8,
              content: '開啟到價通知',
              img: require('../assets/image/4-8.png')
            },
            {
              id: 9,
              content: '將基金商品到價通知選項打勾',
              img: require('../assets/image/4-9.png')
            }
          ]
        },
        {
          step: [
            {
              id: 1,
              content: '行動銀行首頁點選設定',
              img: require('../assets/image/5-2.png')
            },
            {
              id: 2,
              content: '點選基金損益通知設定',
              img: require('../assets/image/5-2.png')
            },
            {
              id: 3,
              content: '點選新增',
              img: require('../assets/image/5-3.png')
            },
            {
              id: 4,
              content: '設定投資類型/基金標的/報酬率上下限/通知起訖日',
              img: require('../assets/image/5-4.png')
            },
            {
              id: 5,
              content: '標的通知設定成功',
              img: require('../assets/image/5-5.png')
            },
            {
              id: 6,
              content: '回行動銀行首頁點選設定，繼續設定系統通知',
              img: require('../assets/image/5-6.png')
            },
            {
              id: 7,
              content: '點選訊息通知設定',
              img: require('../assets/image/5-7.png')
            },
            {
              id: 8,
              content: '開啟到價通知',
              img: require('../assets/image/5-8.png')
            },
            {
              id: 9,
              content: '將基金單筆損益通知選項打勾',
              img: require('../assets/image/5-9.png')
            }
          ]
        }
      ]
    }
  },
  computed: {
    getSliderBlue_1 () {
      return `background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(${this.blue_1}, rgb(0, 159, 232)), color-stop(${this.blue_1}, #a6e0ff))`
    },
    getSliderBlue_2 () {
      return `background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(${this.blue_2}, rgb(0, 159, 232)), color-stop(${this.blue_2}, #a6e0ff))`
    },
    getSliderBlue_3 () {
      return `background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(${this.blue_3}, rgb(0, 159, 232)), color-stop(${this.blue_3}, #a6e0ff))`
    }
  },
  mounted () {
    this.step = 0
    this.tabItem = 1
    this.nextImage()
    this.fetchTab(this.tabItem)
    this.setTimer()
  },
  methods: {
    setTimer () {
      this.startCounter = setInterval(() => {
        if (this.step === this.phoneImage[this.tabItem - 1].step.length) {
          return this.fetchTab(this.tabItem)
        }
        this.nextImage()
      }, 3500)
    },
    nextImage () {
      if (this.step === this.phoneImage[this.tabItem - 1].step.length) return
      this.step++
      this.content = this.phoneImage[this.tabItem - 1].step[this.step - 1].content
      this.thisImage = this.phoneImage[this.tabItem - 1].step[this.step - 1].img
      if (this.step === this.phoneImage[this.tabItem - 1].step.length || this.step === 1) {
        this.bgLine_4 += 1 / 5
        this.bgLine_5 += 1 / 6
        this.bgLine_6 += 0.16
        this.bgLine_9 += 1 / 10
      } else {
        this.bgLine_4 += 1 / 5
        this.bgLine_5 += 1 / 6
        this.bgLine_6 += 1 / 7
        this.bgLine_9 += 1 / 10
      }

      if (this.step > 6) {
        if (this.step === this.phoneImage[this.tabItem - 1].step.length || this.step === 1) {
          this.bgLine_10 += 0.13
        } else {
          this.bgLine_10 += 0.24
        }
      }
    },
    preImage () {
      if (this.step === 1) return
      this.step--
      this.content = this.phoneImage[this.tabItem - 1].step[this.step - 1].content
      this.thisImage = this.phoneImage[this.tabItem - 1].step[this.step - 1].img
    },
    fetchTab (num) {
      this.tabItem = num
      this.step = 1
      this.bgLine_4 = 1 / 6
      this.bgLine_5 = 0.13
      this.bgLine_6 = 0.13
      this.bgLine_9 = 0.13
      this.bgLine_10 = 0.13
      this.stepNumber = this.phoneImage[this.tabItem - 1].step.length
      this.content = this.phoneImage[this.tabItem - 1].step[this.step - 1].content
      this.thisImage = this.phoneImage[this.tabItem - 1].step[this.step - 1].img
    },
    goStep (e) {
      this.step = e.target.innerText.split('')[1]
      this.content = this.phoneImage[this.tabItem - 1].step[this.step - 1].content
      this.thisImage = this.phoneImage[this.tabItem - 1].step[this.step - 1].img
    },
    toggleMenu () {
      this.isOpen = !this.isOpen
    },
    openMbMenu () {
      this.isMbOpen = !this.isMbOpen
    },
    getActiveNumber (val) {
      if (this.step >= val) {
        return 'active_number'
      }
      return 'normal_number'
    },
    goTop () {
      document.body.scrollTop = 0
      document.documentElement.scrollTop = 0
    },
    changeSlider (val) {
      if (val === 1) {
        this.sliderValue_1 = this.value_1
        this.blue_1 = Number(Number(this.sliderValue_1) / 20000)
      } else if (val === 2) {
        this.sliderValue_2 = this.value_2
        this.blue_2 = Number((Number(this.sliderValue_2) - 5) / 7)
      } else if (val === 3) {
        this.sliderValue_3 = this.value_3
        this.blue_3 = Number(Number(this.sliderValue_3) / 40)
      }
    },
    inputSlider (val) {
      if (val === 1) {
        this.value_1 = this.sliderValue_1
        this.blue_1 = Number(Number(this.sliderValue_1) / 20000)
      } else if (val === 2) {
        this.value_2 = this.sliderValue_2
        this.blue_2 = Number((Number(this.sliderValue_2) - 5) / 7)
      } else if (val === 3) {
        this.value_3 = this.sliderValue_3
        this.blue_3 = Number(Number(this.sliderValue_3) / 40)
      }
    },
    newPage (val) {
      if (val === 'fans') {
        window.open('https://www.facebook.com/yuantabank/')
      } else if (val === 'line') {
        window.open('https://line.me/R/ti/p/%40mwr3999i')
      } else if (val === 'ig') {
        window.open('https://www.instagram.com/yuantabank/')
      } else if (val === 'yt') {
        window.open('https://www.youtube.com/channel/UCs72_Ba4-zxCCaeF7zsoAoA')
      } else if (val === 'tg') {
        window.open('https://t.me/yuantabanktw')
      }
    }
  }
}
</script>
<style lang="scss" scoped>
.container-fluid {
    max-width: 1600px;
    margin: 0 auto;
}
.header_bar {
    height: 80px;
    box-shadow: 5px 5px 10px 0 rgba(228, 233, 240, 0.45);
}

.header_flower {
    height: 80px;
    position: absolute;
    right: -100px;
}

@media (max-width: 992px) {
    .header_flower {
        display: none;
    }
}

@media (max-width: 992px) {
    .header_plus {
        display: none;
    }
}

@media (max-width: 576px) {
    .header_plus {
        display: none;
    }
}

.header_item {
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    /*display: block;*/
}

.header_item > li {
    cursor: pointer;
    z-index: 1;
}

@media (max-width: 992px) {
    .header_item {
        display: none;
    }
}

@media (max-width: 576px) {
    .header_item {
        display: none;
    }
}

.menu {
    display: none;
    position: relative;
}

@media (max-width: 992px) {
    .menu {
        display: flex;
    }
}

@media (max-width: 576px) {
    .menu {
        display: block;
    }
}

.menu_list {
    position: absolute;
    width: 100%;
    height: 700px;
    background-color: #ffffff;
    z-index: -1;
    top: -700px;
    left: 0;
    right: 0;
    display: flex;
    align-items: self-start;
    justify-content: center;
}

@media (max-width: 576px) {
    .menu_list {
        position: absolute;
        width: 100%;
        height: 100vh;
        background-color: #ffffff;
        z-index: -1;
        top: -2000px;
        left: 0;
        right: 0;
        display: flex;
        align-items: self-start;
        justify-content: center;
    }
}

.isOpen {
    top: 80px;
    animation: transMenu 0.6s;
}

.arrow {
    cursor: pointer;
}

.list_item {
    width: 300px;
    border-bottom: 1px solid #002d68;
    font-size: 16px;
    letter-spacing: 0.8px;
    color: #092132;
    text-align: left;
}

.item {
    margin-left: 20px;
    display: flex;
    align-items: start;
}

.item > img {
    margin-right: 20px;
}

.item > div {
    width: 166px;
    padding-bottom: 20px;
    border-bottom: 1px solid #d7f1ff;
}

.item:last-child > div {
    border-bottom: none;
}

.pc_menu {
    position: absolute;
    top: 35px;
    right: 0px;
    background-color: #ffffff;
    width: 198px;
    display: none;
}

.pc_menu > li {
    display: flex;
    align-items: center;
    padding: 10px;
    cursor: pointer;
}

.pc_menu > li > div {
    width: 150px;
    border-bottom: 1px solid #d7f1ff;
    font-size: 16px;
    line-height: 1.88;
    letter-spacing: 0.8px;
    color: #044ba8;
}

.pc_menu > li > img {
    margin: 5px 0;
    margin-left: 10px;
    margin-right: 20px;
}

.openMenu {
    display: block;
}

.banner {
    position: relative;
    height: 910px;
    max-height: 100%;
    display: block;
}

@media (max-width: 1200px) {
  .banner {
    height: 470px;
  }
}

@media (max-width: 992px) {
    .banner {
        display: none;
    }
}

@media (max-width: 576px) {
    .banner {
        display: none;
    }
}

.banner_mb {
    display: none;
}

@media (max-width: 992px) {
    .banner_mb {
        position: relative;
        height: 739px;
        max-height: 100%;
        display: block;
    }
}

@media (max-width: 576px) {
    .banner_mb {
        position: relative;
        height: 600px;
        max-height: 100%;
        display: block;
    }
}

.scene {
    position: absolute;
    width: 100%;
    top: 80px;
    left: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(var(--translateY));
    will-change: transform;
}

@media (max-width: 992px) {
  .scene {
    top: 80px;
  }
}

.sidebar_1 {
  position: absolute;
  right: 300px;
  top: 350px;
  height: 90px;
  width: 90px;
  background-color: #ffffff;
  cursor: pointer;
}

@media (max-width: 1200px) {
  .sidebar_1 {
    right: 200px;
    top: 300px;
  }
}

.sidebar_2 {
  position: absolute;
  right: 300px;
  top: 450px;
  height: 90px;
  width: 90px;
  background-color: #ffffff;
  cursor: pointer;
}

@media (max-width: 1200px) {
  .sidebar_2 {
    right: 200px;
    top: 400px;
  }
}

.sidebar_text {
  font-size: 16px;
  font-weight: 500;
  line-height: 1.88;
  letter-spacing: 0.8px;
  color: #51a8ff;
}

.second_cloud {
    position: relative;
    width: 100%;
}

.sec_1 {
    width: 100%;
}

@media (max-width: 992px) {
    .sec_1 {
        width: 300px;
        height: 175px;
    }
}

@media (max-width: 576px) {
    .sec_1 {
        width: 100%;
        height: 100%
    }
}

.save_sec {
    width: 100%;
}

@media (max-width: 992px) {
  .save_sec {
        width: 40%;
    }
}

@media (max-width: 576px) {
    .save_sec {
        width: 100%;
        margin-top: 20px;
    }
}

.step_1 {
    position: relative;
    top: -300px;
    text-align: center;
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #ffffff;
    padding: 80px;
    width: 70%;
    margin: auto;
}

@media (max-width: 1200px) {
  .step_1 {
    position: relative;
    top: -100px;
    text-align: center;
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #ffffff;
    padding: 80px;
    width: 70%;
    margin: auto;
}
}

@media (max-width: 992px) {
    .step_1 {
        top: -88px;
        padding: 20px;

    }
}

@media (max-width: 576px) {
    .step_1 {
        padding: 20px;
        top: -83px;
        width: 100%;
    }
}

.step_1_title {
    width: 60%;
    background-image: linear-gradient(to top, #002d68 100%, #104c9c 0%);
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    text-align: center;
    color: #fff;
    margin: auto;
    padding: 10px 0;
    position: absolute;
    top: -50px;
    left: 50%;
    transform: translate(-50%, 5%);
}

@media (max-width: 992px) {
    .step_1_title {
        width: 40%;
        font-size: 24px;
    }
}

@media (max-width: 576px) {
    .step_1_title {
        width: 80%;
        font-size: 24px;
    }
}

.step_1_content {
    font-size: 22px;
    font-weight: 500;
    line-height: 1.59;
    letter-spacing: 2.2px;
    text-align: center;
    color: #002d68;
}

@media (max-width: 992px) {
    .step_1_content {
        font-size: 18px;
    }
}

@media (max-width: 576px) {
    .step_1_content {
        font-size: 18px;
    }
}

.step_1_by {
    font-size: 18px;
    font-weight: 500;
    line-height: 1.94;
    letter-spacing: 1.8px;
    text-align: center;
    color: #002d68;
    margin-top: 30px;
    background-color: #ffffff;
    z-index: 1;
    width: 150px;
    position: relative;
    left: 50%;
    transform: translate(-50%, 0);
}

@media (max-width: 992px) {
    .step_1_by {
        font-size: 16px;
        width: 150px;
    }
}

.quota_right {
    font-family: RussoOne;
    font-size: 50px;
    line-height: 0.7;
    letter-spacing: 5px;
    text-align: center;
    color: #ff9f59;
    position: relative;
    top: 50px;
}

.quota_left {
    font-family: RussoOne;
    font-size: 50px;
    line-height: 0.7;
    letter-spacing: 5px;
    text-align: center;
    color: #ff9f59;
}

.dash_line {
    position: relative;
    width: 300px;
    top: 50px;
    left: 50%;
    transform: translate(-50%, -50%);
}

.bg_light {
    background-color: #f6fcff ;
}

.container {
    margin: 0 auto;
    position: relative;
    top: -170px;
}

@media (max--width: 992px) {
    .container {
        margin: 0 auto;
        position: relative;
        top: -100px;
    }
}

@media (max-width: 576px) {
    .container {
        margin: 0 auto;
        position: relative;
        top: -16px;
    }
}

.save_text {
    font-size: 18px;
    line-height: 1.94;
    letter-spacing: 0.9px;
    text-align: left;
    color: #021835;
}

@media (max-width: 992px) {
  .save_text {
    font-size: 16px;
    line-height: 1.56;
    letter-spacing: 0.8px;
    text-align: left;
    color: #021835;
  }
}

@media (max-width: 576px) {
    .save_text {
        font-size: 16px;
        line-height: 1.56;
        letter-spacing: 0.8px;
    }
}

.step_2 {
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    text-align: center;
    color: #002d68;
    margin-top: 150px;
    margin-bottom: 80px;
}

@media (max-width: 992px) {
  .step_2 {
    font-size: 22px;
    font-weight: bold;
    letter-spacing: 2.2px;
    text-align: center;
    color: #002d68;
  }
}

@media (max-width: 576px) {
  .step_2 {
    font-size: 22px;
    margin-top: 80px;
}
}

.tips_card {
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
    padding: 50px;
    width: 30%;
    display: grid;
    align-content: center;
    justify-items: center;
}

@media (max-width: 992px) {
    .tips_card {
        padding: 10px;
        width: 32%;
        height: 360px;
    }
}

@media (max-width: 576px) {
    .tips_card {
        padding: 10px;
        width: 100%;
        margin-bottom: 30px;
    }
}

.tips_title {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    text-align: left;
    color: #021835;
    padding-top: 150px;
    padding-bottom: 80px;
}

@media (max-width: 992px) {
    .tips_title {
        padding-top: 30px;
        padding-bottom: 30px;
    }
}

@media (max-width: 576px) {
    .tips_title {
        padding-top: 30px;
        padding-bottom: 30px;
    }
}

.tips_content {
    font-size: 18px;
    line-height: 1.94;
    letter-spacing: 0.9px;
    text-align: left;
    color: #021835;
}

.shine {
    position: relative;
    top: -20px;
}

.step_3 {
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    text-align: center;
    color: #002d68;
    padding-top: 150px;
    padding-bottom: 80px;
}

@media (max-width: 992px) {
    .step_3 {
      font-size: 22px;
      font-weight: bold;
      letter-spacing: 2.2px;
      text-align: center;
      color: #002d68;
    }
}

@media (max-width: 576px) {
    .step_3 {
        font-size: 24px;
        padding-top: 80px;
        padding-bottom: 80px;
    }
}

.step_list {
    margin-left: 10px;
    text-align: left;
    //margin-bottom: 10px;
}

.step_tab {
    background-image: linear-gradient(to top, #51a8ff 100%, #94c9ff 0%);
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    text-align: left;
    color: #fff;
    width: 150px;
    text-align: center;
    padding: 10px 0;
    position: absolute;
    top: -30px;
    left: 50%;
    transform: translate(-50%, 0%);
}

.tab_card {
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
    padding: 50px;
    position: relative;
}

@media (max-width: 992px) {
    .tab_card {
        width: 48%;
        padding: 20px;
        padding-top: 40px;
    }
}

@media (max-width: 576px) {
    .tab_card {
        width: 95%;
        margin: auto;
        margin-bottom: 50px;
    }
}

.flowers  {
    position: relative;
    top: 100px;
    left: 50%;
    transform: translate(-50%, 0%);
    width: 100%;
}

@media (max-width: 992px) {
    .flowers  {
        top: 52px
    }
}

@media (max-width: 576px) {
    .flowers  {
        top: 26px;
    }
}

.darkblue {
    width: 100%;
    position: relative;
}

.bg-darkBlue {
   background-color: #c2e6ff;
}

.step_4 {
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
}

.financial_method_title {
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    text-align: left;
    color: #fff;
    padding: 13px 66px;
    background-image: linear-gradient(to top, #002d68 100%, #104c9c 0%);
    width: 400px;
    text-align: center;
    position: relative;
    top: -30px;
    left: 50%;
    transform: translate(-50%, 0%);
}

@media (max-width: 992px) {
  .financial_method_title {
    font-size: 24px;
    font-weight: bold;
    letter-spacing: 2.4px;
    text-align: center;
    color: #fff;
  }
}

@media (max-width: 576px) {
    .financial_method_title {
        font-size: 24px;
        width: 300px;
        padding: 13px 30px;
        text-align: center;
    }
}

.financial_method_subtitle {
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    text-align: center;
    color: #002d68;
    padding-top: 50px;
    padding-bottom: 100px;
}

@media (max-width: 576px) {
    .financial_method_subtitle {
        font-size: 22px;
        padding: 50px 30px;
    }
}

.invest_title {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    text-align: left;
    color: #021835;
    padding-bottom: 30px;
}

@media (max-width: 576px) {
    .invest_title {
        font-size: 18px;
        text-align: center;
    }
}

.pig {
    width: 100%;
}

.invest_text {
    font-size: 18px;
    line-height: 1.94;
    letter-spacing: 0.9px;
    text-align: left;
    color: #021835;
}

@media (max-width: 576px) {
    .invest_text {
        font-size: 16px;
        padding: 0 20px;
    }
}

.invest_button {
    margin-top: 20px;
    width: 150px;
    color: #ffffff;
    padding: 10px 30px;
    cursor: pointer;
    border-radius: 30px;
    box-shadow: 10px 10px 20px 0 #ffebdd;
    background-image: linear-gradient(to bottom, #ffb36c 0%, #f6733b 100%);
}

.invest_button:hover {
    background-image: linear-gradient(to bottom, #ff8e26 0%, #ff4d00 100%);
}

@media (max-width: 576px) {
    .invest_button {
        width: 150px;
        margin: auto;
    }
}

.feature_card {
    width: 40%;
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
    padding: 20px;
}

@media (max-width: 992px) {
    .feature_card {
        width: 48%;
    }
}

@media (max-width: 576px) {
    .feature_card {
        width: 100%;
        margin-bottom: 30px;
    }
}

.feature {
    padding-left: 20px;
}

.feature_log {
    font-size: 14px;
    letter-spacing: 1.4px;
    text-align: left;
    color: #044ba8;
}

.feature_title {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    text-align: left;
    color: #021835;
    padding-bottom: 20px;
}

.feature_content {
    font-size: 16px;
    line-height: 1.88;
    letter-spacing: 0.8px;
    text-align: left;
    color: #021835;
}

.calculation {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #fff;
    padding: 20px 0;
    background-image: linear-gradient(to top, #51a8ff 100%, #94c9ff 0%);
}

.calculation_card {
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
}

.step_calculation {
    width: 80%;
    margin: auto;
    padding-bottom: 50px;
}

@media (max-width: 992px) {
    .step_calculation {
        width: 95%;
        margin: auto;
        padding-bottom: 50px;
    }
}

@media (max-width: 576px) {
    .step_calculation {
        width: 100%;
        margin: auto;
        padding-bottom: 50px;
    }
}

.calculation_card > .card_title {
    font-size: 18px;
    font-weight: 500;
    line-height: 1.94;
    letter-spacing: 0.9px;
    text-align: center;
    color: #021835;
    padding: 30px 0;

}

@media (max-width: 576px) {
    .calculation_card > .card_title {
        font-size: 16px;
        padding: 30px 50px;

    }
}

.tab_list {
    padding: 40px 0;
    border-bottom: 1px solid #d7f1ff;
}

@media (max-width: 992px) {
    .tab_list {
        padding: 20px 0;
    }
}

@media (max-width: 576px) {
    .tab_list {
        padding: 20px 0;
    }
}

.items_title {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #021835;
}

@media (max-width: 992px) {
    .items_title {
        font-size: 18px;
    }
}

@media (max-width: 576px) {
    .items_title {
        display: grid;
        font-size: 18px;
    }
}

.items_title > span {
    font-size: 16px;
    font-weight: 500;
    line-height: 1.88;
    letter-spacing: 0.8px;
    text-align: left;
    color: #b5c3c7;
}

@media (max-width: 992px) {
    .items_title > span {
        font-size: 14px;
    }
}

@media (max-width: 576px) {
    .items_title > span {
        font-size: 14px;
    }
}

.input_style {
    border: solid 1px #d7f1ff;
    height: 50px;
    font-size: 26px;
    font-weight: 900;
    letter-spacing: 2.2px;
    color: #002d68;
    text-align: right;
    padding-right: 20px;
}

@media (max-width: 576px) {
    .input_style {
        font-size: 22px;
        border: solid 1px #d7f1ff;
        height: 50px;
        width: 100px;
    }
}

.number_bar {
    font-size: 16px;
    line-height: 1.88;
    letter-spacing: 0.8px;
    color: #b5c3c7;
}

@media (max-width: 576px) {
    .number_bar {
        font-size: 14px;
    }
}

.unit {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #021835;
}

.calculation_total {
    padding-left: 0;
}

.total_card {
    width: 30%;
    padding: 20px;
    text-align: center;
    box-shadow: 3px 3px 5px 0 #f1faff;
    background-image: linear-gradient(to bottom, #f2fbff 0%, #d6f0ff 100%);
}

@media (max-width: 576px) {
    .total_card {
        width: 80%;
        margin: auto;
        margin-bottom: 20px;
    }
}

.total_title {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #021835;
}

.dashed_dollar {
    width: 60%;
    border-bottom: 1px solid #51a8ff ;
}

.total_unit {
    font-size: 18px;
    font-weight: 500;
    line-height: 1.94;
    letter-spacing: 0.9px;
    color: #021835;
}

.illustrate {
    font-size: 14px;
    line-height: 1.79;
    letter-spacing: 0.7px;
    color: #b5c3c7;
    padding-top: 40px;
    padding-bottom: 50px;
    text-align: left;
}

.step_5 {
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
    width: 50%;
    margin: auto;
    padding-bottom: 30px;
    margin-bottom: 100px;
}

@media (max-width: 992px) {
  .step_5 {
    width: 80%;
  }
 }

@media (max-width: 576px) {
    .step_5 {
        width: 90%;
    }
}

.save_title {
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    padding: 13px 66px;
    color: #fff;
    background-image: linear-gradient(to top, #002d68 100%, #104c9c 0%);
    width: 400px;
    text-align: center;
    position: relative;
    top: -20px;
    left: 50%;
    transform: translate(-50%, 0%);
}

@media (max-width: 992px) {
  .save_title {
      font-size: 24px;
      font-weight: bold;
      letter-spacing: 2.4px;
      text-align: center;
      color: #fff;
  }
}

@media (max-width: 576px) {
    .save_title {
        font-size: 24px;
        padding: 13px 30px;
        width: 300px;
    }
}

.discount_text {
    font-size: 28px;
    font-weight: bold;
    line-height: 1.25;
    letter-spacing: 4.2px;
    color: #1c8af8;
    text-align: center;
}

.discount_time {
    font-size: 19px;
    line-height: 1.84;
    letter-spacing: 1.9px;
    color: #002d68;
    text-align: center;
}

.discount_time > span {
    font-size: 18px;
    font-weight: 500;
    letter-spacing: 1.8px;
}

.save {
    width: 45%;
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
    position: relative;
    padding-bottom: 40px;
}

@media (max-width: 992px) {
    .save {
        width: 49.5%;
    }
}

@media (max-width: 576px) {
    .save {
        width: 100%;
        padding-bottom: 40px;
    }
}

.save_tab {
    width: 200px;
    margin: auto;
    padding: 10px 0;
    text-align: center;
    color: #ffffff;
    position: relative;
    top: -30px;
    background-image: linear-gradient(to top, #51a8ff 100%, #94c9ff 0%);
}

.save_tab_title {
    font-size: 18px;
    line-height: 1.94;
    letter-spacing: 0.9px;
    text-align: center;
    color: #021835;
}

.save_slogan {
    font-size: 20px;
    font-weight: bold;
    line-height: 1.75;
    letter-spacing: 2px;
    text-align: center;
    color: #ff9f59;
    margin: 20px 0;
}

.save_tab_subtitle {
    width: 80%;
    margin: auto;
    padding: 10px;
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #021835;
    padding-left: 30px;
    background-image: linear-gradient(to bottom, #f2fbff 0%, #d6f0ff 100%);
}

@media (max-width: 992px) {
    .save_tab_subtitle {
        width: 95%;
    }
}

@media (max-width: 576px) {
    .save_tab_subtitle {
        width: 95%;
    }
}

.save_tab_content {
    width: 80%;
    margin: auto;
    padding: 20px;
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
}

@media (max-width: 992px) {
    .save_tab_content {
        width: 95%;
        padding: 10px;
    }
}

@media (max-width: 576px) {
    .save_tab_content {
        width: 95%;
        padding: 10px;
        margin-bottom: 30px;
    }
}

.save_list {
    border-bottom: 1px solid #d7f1ff;
}

.save_list:last-child {
    border-bottom: none;
}

.save_list_title {
    padding-left: 10px;
    text-align: left;
}

@media (max-width: 992px) {
    .save_list_title {
        font-size: 16px;
        line-height: 1.56;
        letter-spacing: 0.8px;
        color: #021835;
    }
}

.link_icon {
    cursor: pointer;
}

.link_show {
    cursor: pointer;
    display: block;
}

.link_active {
    display: none;
}

.link_none {
    display: none;
}

.empty_parameter {
    height: 81px;
}

@media (max-width: 992px) {
    .empty_parameter {
        height: 28px;
    }
}

.remark {
    font-size: 16px;
    line-height: 1.25;
    letter-spacing: 0.8px;
    color: #b5c3c7;
    position: relative;
    text-align: left;
    left: 20px;
    top: -10px
}

@media (max-width: 992px) {
    .remark {
        font-size: 14px;
        line-height: 1.25;
        letter-spacing: 0.8px;
        color: #b5c3c7;
        position: relative;
        left: 10px;
        top: 10px
    }
}

@media (max-width: 576px) {
    .remark {
        font-size: 14px;
        line-height: 1.25;
        letter-spacing: 0.8px;
        color: #b5c3c7;
        position: relative;
        left: 10px;
        top: 10px
    }
}

.step_6 {
    width: 700px;
    margin: auto;
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    text-align: center;
    color: #fff;
    padding: 13px 70px 13px 68px;
    background-image: linear-gradient(to top, #002d68 100%, #104c9c 0%);
}

@media (max-width: 992px) {
  .step_6 {
    font-size: 24px;
    font-weight: bold;
    letter-spacing: 2.4px;
    text-align: center;
    color: #fff;
  }
}

@media (max-width: 576px) {
    .step_6 {
        text-align: center;
        width: 300px;
        font-size: 24px;
        padding: 13px 20px;
    }
}

.tab {
    margin-top: 50px;
    margin-bottom: 0;
    width: 100%;
    padding-left: 0;
}

@media (max-width: 576px) {
    .tab {
       overflow: scroll;
    }
}

.tab > li {
    width: calc(100% / 5);
    text-align: center;
    padding: 20px 0;
}

.tab > li > div {
    border-left: 1px solid #ffffff;
}

.tab > li:first-child > div {
    border-left: none;
}

.active_tab {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #021835;
    background-color: #ffffff;
}

@media (max-width: 992px) {
    .active_tab {
        font-size: 18px;
    }
}

.normal_tab {
    cursor: pointer;
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #ffffff;
    background-image: linear-gradient(to top, #208fff 100%, #71b8ff 0%);
}

@media (max-width: 992px) {
    .normal_tab {
        font-size: 18px;
    }
}

.single_subscription {
    background-color: #ffffff;
    padding-bottom: 50px;
    position: relative;
    z-index: 1;
}

.single_title {
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 3px;
    text-align: center;
    color: #002d68;
    padding-top: 100px;
}

@media (max-width: 992px) {
    .single_title {
        font-size: 22px;
        padding-top: 50px;
    }
}

@media (max-width: 576px) {
    .single_title {
        padding-top: 30px;
    }
}

.single_subtitle {
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    text-align: center;
    color: #021835;
    padding: 30px 0;
    margin-bottom: 30px;
}

.four_step {
    width: 24%;
    margin: auto;
    position: relative;
    top: -30px;
}

.four_step > li:after {
    content: "";
    position: absolute;
    width: 82%;
    height: 3px;
    top: 28px;
    left: 9%;
    z-index: -1;
    background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(var(--bgImage), #044ba8), color-stop(var(--bgImage), #91bffb))
}

.five_step {
    width: 30%;
    margin: auto;
    position: relative;
    top: -30px;
}

.five_step > li:after {
    content: "";
    position: absolute;
    width: 86%;
    height: 3px;
    top: 28px;
    left: 7%;
    z-index: -1;
    background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(var(--bgImage), #044ba8), color-stop(var(--bgImage), #91bffb))
}

.six_step {
    width: 38%;
    margin: auto;
    position: relative;
    top: -30px;
}

.six_step > li:after {
    content: "";
    position: absolute;
    width: 100%;
    height: 3px;
    background-color: #91bffb;;
    top: 80px;
    left: 0%;
    z-index: -1;
    background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(var(--bgImage), #044ba8), color-stop(var(--bgImage), #91bffb))
}

.nine_step {
    width: 38%;
    margin: auto;
    position: relative;
    top: -30px;
}

.nine_step > li:after {
    content: "";
    position: absolute;
    width: 88%;
    height: 3px;
    background-color: #91bffb;;
    top: 28px;
    left: 6%;
    z-index: -1;
    background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(var(--bgImage), #044ba8), color-stop(var(--bgImage), #91bffb))
}

.nine_2_step {
    width: 18%;
    margin: auto;
    position: relative;
    top: -30px;
    margin-top: 30px;
}
.nine_2_step > li:after {
    content: "";
    position: absolute;
    width: 75%;
    height: 3px;
    background-color: #91bffb;;
    top: 28px;
    left: 12%;
    z-index: -1;
    background-image: -webkit-gradient(linear, 0% 100%, 100% 100%, color-stop(var(--bgImage), #044ba8), color-stop(var(--bgImage), #91bffb))
}

.number_step > li:first-child:after {
    content: none;
}

@media (max-width: 576px) {
    .number_step {
        width: 300px;
        margin: auto;
        position: relative;
        top: -20px;
    }
}

.number_step > .active_number {
    font-size: 22px;
    letter-spacing: 2.2px;
    color: #ffffff;
    height: 60px;
    width: 60px;
    border-radius: 45px;
    font-weight: 900;
    box-shadow: 3px 3px 10px 0 rgba(188, 222, 255, 0.35);
    background-image: linear-gradient(to top, #51a8ff 100%, #94c9ff 0%);
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}

@media (max-width: 576px) {
    .number_step > .active_number {
        font-size: 17.6px;
        height: 40px;
        width: 40px;
        border-radius: 45px;
    }
}

.number_step > .normal_number {
    font-size: 22px;
    letter-spacing: 2.2px;
    color: #91bffb;
    height: 60px;
    width: 60px;
    border-radius: 45px;
    box-shadow: 3px 3px 10px 0 rgba(188, 222, 255, 0.35);
    background-image: linear-gradient(to bottom, #f2fbff 0%, #d6f0ff 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    font-weight: 900;
}

.normal_number:hover {
    font-size: 22px;
    font-weight: 900;
    letter-spacing: 2.2px;
    color: #044ba8;
}

@media (max-width: 576px) {
    .number_step > .normal_number {
        font-size: 17.6px;
        height: 40px;
        width: 40px;
        border-radius: 45px;
    }
}

.phone {
    position: relative;
    height: 430px;
    width: 200px;
    overflow-y: scroll;
    border-radius: 17px;
    box-shadow: 3px 3px 10px 0 #BCDEFF;
}

@media (max-width: 576px) {
    .phone {
         text-align: center;
         margin: auto;
    }
}

.phone_out {
    position: sticky;
    left: 0;
    top: -3px;
}

.phone_body {
    position: absolute;
    top: 3px
}

.bubble {
    position: relative;
    top: -90px;
    left: -18px;
}

@media (max-width: 576px) {
    .bubble {
        position: relative;
        top: -13px;
        left: 10px;
    }
}

.bubble_pc {
    display: block;
}

@media (max-width: 576px) {
    .bubble_pc {
        display: none;
    }
}

.bubble_mb {
    display: none;
}

@media (max-width: 576px) {
    .bubble_mb {
        display: block;
    }
}

.bubble_title {
    font-size: 22px;
    letter-spacing: 2.2px;
    font-weight: 900;
    color: #044ba8;
    position: absolute;
    top: 10px;
    left: 63px;
}

@media (max-width: 576px) {
    .bubble_title {
        top: 28px;
        left: 12px;
    }
}

.bubble_content {
       width: 330px;
    font-size: 18px;
    line-height: 1.94;
    letter-spacing: 0.9px;
    color: #021835;
    position: absolute;
    top: 37px;
    left: 50px;
    text-align: left;
    padding: 0 10px;
}

@media (max-width: 576px) {
    .bubble_content {
        top: 53px;
        left: 0px;
    }
}

.step_button {
    color: #ffffff;
    width: 200px;
    padding: 15px 50px;
    border-radius: 30px;
    box-shadow: 10px 10px 20px 0 #ffebdd;
    background-image: linear-gradient(to bottom, #ffb36c 0%, #f6733b 100%);
    position: relative;
    left: 100px;
    top: 100px;
    cursor: pointer;
}

.step_button:hover {
    background-image: linear-gradient(to bottom, #ff8e26 0%, #ff4d00 100%);
}

@media (max-width: 576px) {
    .step_button {
        left: 60px;
        top: 36px;
    }
}

.web {
    position: absolute;
    top: -500px;
    left: -116px;
}

@media (max-width: 992px) {
    .web {
        top: -631px;
    }
}

.third_title {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #021835;
    text-align: center;
    padding-bottom: 50px;
}

.third_circle {
    height: 160px;
    width: 160px;
    border-radius: 50%;
    padding: 40px;
    box-shadow: 10px 10px 30px 0 rgba(228, 233, 240, 0.45);
    background-color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
}

@media (max-width: 576px) {
    .third_circle {
        height: 100px;
        width: 100px;
    }

    .third_circle > img {
        height: 48px;
        width: 48px;
    }
}

.third_icon {
  cursor: pointer;
}

@media (max-width: 576px) {
    .third_icon {
        display: grid;
        align-content: center;
        justify-items: center;
    }
}

@media (max-width: 768px) {
    .third_icon {
        display: grid;
        align-content: center;
        justify-items: center;
    }
}

@media (max-width: 992px) {
    .third_step {
        column-count: 3;

    }
}

.third_text {
    font-size: 16px;
    line-height: 1.88;
    letter-spacing: 0.8px;
    text-align: center;
    color: #021835;
}

@media (max-width: 576px) {
    .third_circle {
        font-size: 14px;
    }
}

.notice {
    position: relative;
    top: -170px;
}

@media (max-width: 992px) {
    .notice {
        top: -50px;
    }
}

@media (max-width: 576px) {
    .notice {
        top: -50px;
    }
}

.notice_title {
    font-size: 22px;
    font-weight: bold;
    line-height: 1.59;
    letter-spacing: 2.2px;
    color: #021835;
    text-align: center;
}

@media (max-width: 576px) {
    .notice_title {
        font-size: 16px;
    }
}

.notice_content {
    font-size: 16px;
    line-height: 1.88;
    letter-spacing: 0.8px;
    color: #021835;
}

@media (max-width: 576px) {
    .notice_content {
        font-size: 14px;
    }
}

.notice_content_title {
    font-size: 18px;
    font-weight: 500;
    line-height: 1.94;
    letter-spacing: 0.9px;
    text-align: left;
    color: #021835;
}

ol li {
  text-align: left;
}

ol > div {
  text-align: left;
}

.footer_address {
    font-size: 16px;
    font-weight: bold;
    line-height: 1.88;
    letter-spacing: 0.8px;
    text-align: center;
    color: #021835;
    margin-top: 30px;
}

.footer {
    height: 150px;
    width: 100%;
    background-color: #044ba8;
    text-align: center;
    display: grid;
    align-content: center;
    justify-items: center;
    color: #ffffff;
}

@media (max-width: 576px) {
    .footer {
       font-size: 14px;
       text-align: left;
       padding: 0 20px;
    }
}

.open_account {
  display: none;
}

@media (max-width: 992px) {
  .open_account {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
}

@media (max-width: 576px) {
  .open_account {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
}

.open_account > li {
  width: 50%;
  margin: 20px 0;
  cursor: pointer;
}

.open_account > li:first-child {
  border-right: 1px solid #d7f1ff;
}

.open_account > li > div > img {
  height: 35px;
  width: 35px;
  margin-right: 10px;
}

.account_text {
  font-size: 16px;
  font-weight: 500;
  line-height: 1.88;
  letter-spacing: 0.8px;
  text-align: left;
  color: #51a8ff;
}

.to_top {
    position: fixed;
    right: 20px;
    bottom: 20px;
    cursor: pointer;
    z-index: 1;
}

.to_top > div {
    font-size: 22px;
    letter-spacing: 2.2px;
    text-align: center;
    color: #91bffb;
}

.range-slider__range {
    -webkit-appearance: none;
    -moz-appearance: none;
    width: 100%;
    height: 10px;
    border-radius: 5px;
    background: #fff;
    outline: none;
    padding: 0;
    margin: 0;
    cursor: pointer;
}

.range-slider__range::-webkit-slider-thumb {
    width: 38px;
    height: 38px;
    border-radius: 50%;
    -webkit-appearance: none;
    /*background: red;*/
    background-image: url(../assets/image/money.png);
    background-size: contain;
}

@media (max-width: 576px) {
  .range-slider__range::-webkit-slider-thumb {
    width: 25px;
    height: 25px;
  }
}

.next_icon {
    cursor: pointer;
    padding-left: 30px;
}

.pre_icon {
    cursor: pointer;
    padding-right: 50px;
}

@keyframes transMenu {
    0% {
      transform: translateY(-800px);
    }
    100% {
      transform: translateY(80);
    }
}

input::-webkit-outer-spin-button, input::-webkit-inner-spin-button {
  -webkit-appearance: none;
}

input[type="number"] {
  -moz-appearance: textfield;
}

</style>
