---
layout: clean
title:  "Создание корпоративного сайта"
permalink: pretty
breadcrumb: Создание корпоративного сайта
---
<div class="maxcnt comet__bg">
      <header class="page_header">
        <div class="container">
          <div class="col-md-8">
            <h1 class="page_title white">{{ page.title }}</h1>
          </div>
          <div class="col-md-4">
    <ol class="breadcrumb">
    <li><a href="{{ site.baseurl }}/">Главная</a></li>
    {% capture page_url_without_index_html %}{{ page.url | remove: "/index.html" }}{% endcapture %}
    {% assign splitted_url_parts = page_url_without_index_html | split: '/' %}
    {% capture forLoopMaxInt %}{{ splitted_url_parts.size | minus:1 }}{% endcapture %}
    {% for i in (1..forLoopMaxInt) %}
        {% capture current_breadcrumb_url %}{{next_prepender}}/{{ splitted_url_parts[i] }}/index.html{% endcapture %}
        {% capture current_breadcrumb_md_url %}{{next_prepender}}/{{ splitted_url_parts[i] }}/{% endcapture %}
        {% capture next_prepender %}{{next_prepender}}/{{ splitted_url_parts[i] }}{% endcapture %}
        {% for breadcrumb_page in site.pages %}
            {% if current_breadcrumb_url == breadcrumb_page.url or current_breadcrumb_md_url == breadcrumb_page.url  %}
                <li {% if i == forLoopMaxInt %}class="active"{% endif %}>
        {% capture breadcrumb_page_page_url_without_index_html %}{{ breadcrumb_page.url | remove: "index.html" }}{% endcapture %}
                    <a href="{{ site.baseurl }}{{breadcrumb_page_page_url_without_index_html}}">{{breadcrumb_page.breadcrumb}}</a>
                </li>
            {% endif %}
        {% endfor %}
    {% endfor %}
    </ol>
          </div>
        </div>
      </header>
<section class="corporate_hero wow fadeIn" data-wow-duration="2s">
  <div class="container">
    <div class="col-md-7">
      <div class="corporate_hero__title">
        <p class="white">Мы разрабатываем корпоративные сайты, главная цель которых:</p>
        <h2 class="white text-thin ">Обеспечить вашему бизнесу стабильный поток клиентов за рациональные средства.</h2>
        <a href="#get_commercial" class="dashed_link">Оставить заявку на коммерческое предложение</a>
      </div>
    </div>
  </div>
</section>
</div>

<div class="maxcnt">

<section class="page_section">
  <div class="page_section__title">
    <h3 class="text-center">Ключевые моменты</h3>
  </div>
  <div class="container">
  		<div class="row">
  			<div class="col-md-4 feature_item">
  				<span class="feature_icon"><img src="{{site.baseurl}}/img/web_design_icon.png" alt="продающий дизайн сайта"></span>
  				<h4>Уникальный, индивидуальный и продающий дизайн сайта</h4>
  				<p>В работе над дизайн-проектом корпоративного сайта мы опираемся на акцидентные цвета компании, 
стараемся максимально эргономично организовать пространство и сделать его визуальную часть будущего функционала максимально доступной для каждого посетителя.</p>
  			</div>
  			<div class="col-md-4 feature_item">
  				<span class="feature_icon"><img src="{{site.baseurl}}/img/responsive_icon.png" alt="адаптивный дизайн"></span>
  				<h4>Адаптация под все типы устройств:
ПК, планшеты и смартфоны</h4>
  				<p>Сегодня, в эру гаджетов доступность веб-сайта с 
различных устройств играет важную роль для бизнеса, поэтому мы делаем большой акцент на разработке адаптивного дизайна сайта.</p>  				
  			</div>
  			<div class="col-md-4 feature_item">
  				<span class="feature_icon"><img src="{{site.baseurl}}/img/fast_icon.png" alt="быстрая разработка проекта"></span>
  				<h4>Быстрая скорость разработки проекта и
запуск в кротчайшие сроки</h4>
  				<p>Слаженная команда профессионалов нашего агентства использует передовые технологии для того, чтобы 
разработка проекта происходила в предельно сжатые сроки.</p>  				
  			</div>
  		</div>
  		<hr>  		
  		<div class="row">
  			<div class="col-md-4 feature_item">
  				<span class="feature_icon"><img src="{{site.baseurl}}/img/cms_icon.png" alt="Удобная и безопасная система 
управления сайтом"></span>
  				<h4>Удобная и безопасная система 
управления сайтом</h4>
  				<p>Корпоративный сайт - это всегда много информации: меню, страницы, новости, статьи, каталоги, модули и для того, чтобы легко и быстро управять информацией мы используем инновационную систему управления сайтом, которая без труда позволит управлять таким массивом данных.</p>  				
  			</div>
  			<div class="col-md-4 feature_item">
  				<span class="feature_icon"><img src="{{site.baseurl}}/img/ready_icon.png" alt="готовность к продвижению сайта"></span>
  				<h4>Полная готовность к продвижению и 
посетителям</h4>
  				<p>После реализации проекта, Вы можете быть уверены в том, что сайт полностью готов к продвижению и 
рекламированию в любом виде. Это очень важный аспект так, как не требуется тратить дополнительные деньги на переоптимазацию сайта.</p>  				
  			</div>
  			<div class="col-md-4 feature_item">
  				<span class="feature_icon"><img src="{{site.baseurl}}/img/web_design_icon.png" alt="разработка модулей"></span>
  				<h4>Разработка индивидуальных модулей и нестандартного функционала</h4>
  				<p>Каждый бизнес использует свои уникальные 
инструменты для достижения внимания у клиентов и последующего заключения сделок. Мы готовы предоставит Вам разработку любых нестандартных модулей и интеграций с различными сервисами.</p>  				
  			</div>
  		</div>
  	</div>	
</section>

<section class="page_section">
  <div class="page_section__title">
    <h3 class="text-center">Процесс создания сайта</h3>
  </div>
  <div class="container">
	  <div class="process">
	  	<ul class="process_list no-list clearfix">
	  		<li class="process_list__item wow fadeIn"><h4 class="text-reg">01. Техническое задание</h4><p>С учетом Ваших пожеланий мы составляем техническое задание по которому будем 
	разрабатывать сайт.</p></li>
	  		<li class="process_list__item wow fadeIn" data-wow-delay="1s"><h4 class="text-reg">02. Прототип сайта</h4><p>Делаем ч\б прототип различных шаблонов страниц, 
	согласовываем с вами.</p></li>
	  		<li class="process_list__item wow fadeIn" data-wow-delay="1.5s"><h4 class="text-reg">03. Дизайн сайта</h4><p>Создаем полный дизайн-проект будущего сайта и утверждаем с вами.</p></li>
	  		<li class="process_list__item wow fadeIn" data-wow-delay="2s"><h4 class="text-reg">04. Тех.часть</h4><p>Верстка, програмирование технической части, проверка и отладка всех модулей.</p></li>
	  		<li class="process_list__item wow fadeIn" data-wow-delay="2.5s"><h4 class="text-reg">05. Наполнение, сдача проекта</h4><p>Наполнение контентом, базовая SEO оптимизация под поисковые запросы, сдача проекта.</p></li>
	  	</ul>
	  </div>
  </div>
</section>

<!-- COMMERCIAL PROMO -->
<div class="commercial_promo_box">
	<div class="container">
		<div class="col-md-5 white">
			<h3>Планируете разработку 
корпоративного сайта?</h3>
<p>Оставьте заявку на расчет индивидуального коммерческого предложения - это абсолютно бесплатно!</p>
		</div>

		
			<div class="col-md-7 commercial_promo_box__holder">
				<div class="commercial_promo_box__contact_form">
          <h4>Оставьте заявку на <span class="blue">расчет коммерческого предложения</span> по корпоративному сайту:</h4>
					<form action="">
						<div class="form-group">
              <span class="icon icon-user"></span>
							<input type="text" class="form-control" placeholder="Введите Имя">
						</div>						
						<div class="form-group">
              <span class="icon icon-phone"></span>
							<input type="text" class="form-control" placeholder="Введите контактный телефон">
						</div>						
						<div class="form-group">
              <span class="icon icon-mail"></span>
							<input type="email" class="form-control" placeholder="Введите email для доставки кп">
						</div>
						<input type="submit" action="" class="btn btn-primary" value="Заказать расчет коммерческого">
					</form>
				</div>
			</div>
		
	</div>
</div>

<div class="ipad_com_bg">
<section class="page_section">
  <div class="page_section__title">
    <h3 class="text-center">С нами выгодно работать</h3>
  </div>
  <div class="container">
    <div class="col-md-12">
      <ul class="square_features_l no-list">
        <li class="square_features_l__item wow fadeIn">Высокое <strong>качество и технологичность</strong> будущего проекта;</li>
        <li class="square_features_l__item wow fadeIn" data-wow-delay="0.5s"><strong>Больше сервисов включено</strong> за те же деньги;</li>
        <li class="square_features_l__item wow fadeIn" data-wow-delay="1s">Гарантированное<strong> увеличение продаж;</strong></li>
        <li class="square_features_l__item wow fadeIn" data-wow-delay="1.5s"><strong>Ведение и поддержка сайта</strong>на постоянной основе;</li>
        <li class="square_features_l__item wow fadeIn" data-wow-delay="2s"><strong>Скидка на дальнейшее продвижение</strong>и обслуживание;</li>
        <li class="square_features_l__item wow fadeIn" data-wow-delay="2.5s"><strong>Гарантированные сроки</strong> запуска.</li>
      </ul>
    </div>
  </div>
</section>
</div>

<section class="page_section">
  <div class="page_section__title">
    <h3 class="text-center">Цены на создание корпоративного сайта</h3>
  </div>
  <div class="container">
    <div class="col-md-6">
      <div class="row">
        <div class="col-md-3">
          <img src="{{site.baseurl}}/img/artem_icon.png" alt="Артем Ануфриев">
        </div>
        <div class="col-md-9">
          <div class="speech_bubble">
            <p>Каждый бизнес уникален, как и сайт который его представляет. Мы всегда расчитываем индивидуальное коммерческое предложение с учетом ваших пожеланий и предложенных нами идеями по реализации проекта. Оставьте заявку на расчет коммерческого и мы свяжемся с вами в этот же день!</p>
          </div>
          <p class="small-text">Артем Ануфриев, основатель агентства “NineProject”</p>
        </div>
      </div>
    </div>
    <div class="col-md-6">
      <div class="dashed_container">
        <p>Средняя стоимость разработки корпоративного сайта в нашем агентстве составляет 50.000 руб.</p>
      </div>
    </div>
  </div>
</section>

<section class="page_section">
  <div class="page_section__title">
    <h3 class="text-center">Дополнительные сервисы</h3>
  </div>
  <div class="container">
    <div class="row add_features">
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/domen_mail_icon.png" alt="Почта для домена"></div>
        <h4>Интеграция и настройка почты для домена</h4>
        <p>Настройка корпоративной почты на любом облачном сервисе: Gmail, Yandex, Mail.ru.</p>
      </div>      
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/mailchimp_icon.png" alt="Почтовые рассылки mailchimp"></div>
        <h4>Подключение удобного сервиса для email рассылки</h4>
        <p>Возможность делать  бесплатную 
рассылку писем до 5000 подписчикам.</p>
      </div>      
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/web_stat_icon.png" alt="Яндекс.метрика и Google.Analytics"></div>
        <h4>Профессиональная настройка 
веб-аналитики для сайта</h4>
        <p>Детальная настройка Яндекс.Метрика и Google.Analytics, чтобы отслеживать посещяемость сайта и более глубокие даные о посетителях</p>
      </div>      
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/bitrix_icon.png" alt="Битрикс24"></div>
        <h4>Интеграция сайта с CRM системой «Битрикс-24»</h4>
        <p>Прозрачное управление, статистика продаж, «воронка продаж» и ежемесячные отчеты - в единой системе, доступной из браузера.</p>
      </div>
    </div>    
    <hr>
    <div class="row add_features">
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/1m_support_icon.png" alt="1 месяц бесплатной технической поддержки"></div>
        <h4>Первый месяц поддержки 
бесплатно</h4>
        <p>Обслуживание вашего сайта в течение одного месяца нашими специалистами.</p>
      </div>      
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/expert_consult_icon.png" alt="Консультации экспертов"></div>
        <h4>Консультации экспертов по
интернет-продажам</h4>
        <p>Расскажем о лучших  инструментах и техниках по увилечению продаж с помощью интернета.</p>
      </div>      
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/adwords_icon.png" alt="Google Adwords"></div>
        <h4>Купон на 2.000 руб. на рекламу в Google</h4>
        <p>Легкий путь к первым посетителям!</p>
      </div>      
      <div class="col-md-3">
        <div class="add_feature_icon__container"><img src="{{site.baseurl}}/img/15gbcdn_icon.png" alt="3-х кратное ускорение сайта"></div>
        <h4>3-х кратное ускорение сайта + 15гб дискового места на CDN бесплатно</h4>
        <p>CDN технологии, минимазации файлов позволяют увеличить скорость загрузки страниц практически в 3 раза.</p>
      </div>
    </div>
  </div>
</section>

<div class="lets_get_started">
  <div class="container">
    <div class="col-md-8 col-md-offset-2">
      <h2 class="text-thin text-center">Давайте начнем сотрудничество!</h2>
      <p class="text-center lets_get_started__text">При заказе корпоративного сайта до 25 декабря - <br>вы 
получаете все дополнительные сервисы в подарок!</p>
      <div class="row">
        <div class="col-md-8 col-md-offset-2">
          <div class="ghost_box__form">
              <form action="">
                <div class="form-group">
                  <span class="icon icon-user"></span>
                  <input type="text" class="form-control" placeholder="Введите Имя">
                </div>            
                <div class="form-group">
                  <span class="icon icon-phone"></span>
                  <input type="text" class="form-control" placeholder="Введите контактный телефон">
                </div>            
                <div class="form-group">
                  <span class="icon icon-mail"></span>
                  <input type="email" class="form-control" placeholder="Введите email для доставки кп">
                </div>
                <div class="form-group text-center">
                  <input type="submit" action="" class="btn btn-primary" value="Заказать расчет коммерческого">
                </div>
              </form>        
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

</div>
