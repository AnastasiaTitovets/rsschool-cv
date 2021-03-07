# Anastasia Titovets

Birth date: **22.01.1994**
Phone: **+375 33 671-75-52**
E-mail: **a.v.titovets@mail.ru**

## Short information about me

I'm a сonscientious, disciplined, responsible and proactive person. I don't afraid of work and ready to *eat new knowledge with a big spoon*. I like to work effectively, strive for automatization of monotonus activities to reduce the time on their execution. I have an experience of working in a team. Futhermore, I'm able to negotiate with the clients and close deals.

## My professional skills

HTML, CSS, JavaScript, Jquery, Ajax, PHP, Mysql, Api.

### Some types of tasks I can perform

* Front-End development and modification: creating of HTML markup and its alteration, creating of Schema Org micro-markup, creating of mobile version of sites using media requests;
* Back-End development and modification: adding of new variables/fields in DB tables and creating the functionality to work with them, projecting of new data structures with development of new classes to perform any activities with them on the basis of MVC, development and upgrading CRM for small business management (using PHP, Mysql, HTML, CSS, JS, Jquery), development of a simple site constructor on the basis of PHP language (writing of files, creating of data base, setting of block backgrounds etc.) and some settings.
* Working with API (getting of data from unified state register, implementing of different payment systems to sites, automatic upgrading of currency rates from national bank);
* Working with export/import using CSV data format;
* Working with parcing of products from different sites with the help of Content Downloader X1;
* SEO optimization of sites.

### Additional skills

MS Word, MS Excel, MS Powerpoint, AdobePhotoshop, 1С:Enterprise v. 7.7.

## Work experience

1. May 2017 - September 2017. Worked as a programmist on Individual enterprener Bondarenko A.S.;
2. September 2017 - February 2018. Worked as a programmist on private enterprise "Webstudia 1703";
3. June 2018 - January 2021. Worked as the director (and major programmist) on the enterprise "Webstudia 1703".
## The last projects

* <https://greemdom.by/>
* <http://belseverstroj.by/>
* <http://valmari.by/>
* <http://profibeg.by/>
* <http://dveri.idre.by/>

## Some code examples

### Header block

    <div class="header<?php if (horizontMenuDisable()) : ?> no-menu<?php endif; ?><?php if(isIndex()):?> header-main<?php endif;?>">
	<div class="bottom-bar">
            <div class="centered clearfix"> 		
                <div class="logo-block">
					<a href="<?php echo SITE ?>" class="logo-a-img">
                        <?php echo mgLogo(); ?>
                    </a>
                </div>					
				 <div class="top-search-block">
						<?php layout('search'); ?>
				</div>				 				 
				<div class="top-features">               
                    <?php layout('contacts_address'); ?>    				              
                    <?php layout('contacts'); ?>                               				
                </div>
				<div class="work-hours-block">
				<?php if(trim(MG::getSetting('shopTime')) != ''):?>				
					<div class="work-hours">
							<i class="far fa-clock"></i>
							<div class="hours">
								<?php echo htmlspecialchars_decode(MG::getSetting('shopTime'));?>
							</div>
					</div>
				<?php endif; ?>	
				<?php if(trim(MG::getSetting('shopTime2')) != ''):?>				
					<div class="work-hours">
							<i class="far fa-clock"></i>
							<div class="hours">
								<?php echo htmlspecialchars_decode(MG::getSetting('shopTime2'));?>
							</div>
					</div>
				<?php endif; ?>				    				 
			</div>				
			<div class="header-curr-block">
				<a href="javascript:void(0);" class="currency-btn tool-tip-top" data-toggle="tooltip" title="Выбор валюты"><i class="fas fa-dollar-sign"></i></a>
				<div class="currency-filter-block" style="display: none;">
					<div class="currency-filter-header">Выберите валюту</div>
					<div class="currency-filter-body">
						<?php foreach (MG::getSetting('currencyRate') as $key => $val) {
							echo '<a href="javascript:void(0);" data-currency="'.$key.'">'.$key.'</a>';
						  }  
						?>
					</div>
				</div> 
			</div>			
			<?php layout('cart'); ?>		
            </div>
        </div>
        <div class="top-bar">
            <div class="centered">             				 
                <div class="top-menu-block">                  
                    <?php layout('topmenu'); ?>                   
                    <div class="clear"></div>
                </div>					
                <div class="clear"></div>
            </div>
        </div>     
    </div>
***
### Some CSS instructions

    @media all and (max-width: 1300px) {
    .wrapper .mg-search-block .search-field{
    width: 250px;
    }
    .logo-block,
    .work-hours,
    .top-features{
    margin-right: 30px;
    }
    .favourites-icon-block, .plugins,
    .mg-product-to-compare,
    .wrapper .mg-desktop-cart .cart{
	margin-right: 20px;
    }
    .contacts-callback h3{
    font-size: 20px;
    margin-bottom: 0;
    }
    .contacts-callback p{
    margin-top: 0;
    }
    .catalog-main-menu > li a.category-name{
    font-size: 15px;
    margin: 10px 25px;
    }
    .catalog-main-menu .submenu > li{
    margin: 0 10px 5px 0;
    }
    }
***
### JS code

    $('.open-menu-block-btn').on("click", function (e) {
        e.preventDefault();
        $('.menu-block').toggleClass('open');
        $(this).toggleClass('opened');
    });

    $('.open-search-block-btn').on("click", function (e) {
        e.preventDefault();
        $('.mg-search-block').addClass('open');
    });

    $('.close-search-block-btn').on("click", function (e) {
        e.preventDefault();
        $('.mg-search-block').removeClass('open');
    });

    $('.currency-btn').on("click", function (e) {
        e.preventDefault();
        $('.currency-filter-block').toggleClass('open');
    });

    $('.checkout-btn').on("click", function () {
        var re1 = /^[\w-\.]+@[\w-]+\.[a-z]{2,4}$/i;
        var email = $('.form-list input[name=email]').val();
        if (!re1.test(email) || email == '') {
            alert('Неправильный e-mail адрес.');
            return false;
        }
        var phone = $('.form-list input[name=phone]').val();
        if(phone.length == 0){
            alert('Введите телефон.');
            return false;
        }else{
            ym(11111111, 'reachGoal', 'check');
            gtag('event', 'Оформление заказа', {'event_category': 'checkout', 'event_action': 'check'});
        }
    });
 
## Education

1. September 2011 - June 2015. Belarusian-Russian University. Specialization "Economics and management in enterprise". Qualification "Economist-manager".
2. September 2015 - June 2016. Belarusian-Russian University. Specialization "Economics and management of national economy". Qualification "Master of Economic Sciences".
3. July 2014 - August 2014. Educational center "Mela Rosa". Basic PHP courses.

## Soft skills

### English

Pre-intermediate level.
