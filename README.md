# شکافتن داده‌های دیوار: پروژه‌ای عملی در تحلیل بازار املاک
## مقدمه
در این پروژه جذاب، گامی در مسیر تحلیل داده‌های دنیای واقعی برمی‌داریم. با بهره‌گیری از مجموعه داده ارزشمندی که توسط شرکت محترم دیوار در اختیار ما قرار گرفته است، به کاوش در اعماق اطلاعات نهفته در تبلیغات املاک خواهیم پرداخت. این تجربه عملی، فرصتی بی‌نظیر برای به‌کارگیری دانش و مهارت‌های تحلیل داده در یک سناریوی واقعی را فراهم می‌آورد.
هدف اصلی این پروژه، فراتر از صرفاً انجام تحلیل‌های روتین، بستری برای توانمندسازی علاقه‌مندان به حوزه تحلیل داده و علم داده است. از یک سو، تلاش خواهیم کرد تا مجموعه‌ای از فعالیت‌های کلیدی که یک تحلیلگر داده باید بر آن‌ها مسلط باشد را به صورت عملی تجربه کنیم. این شامل مراحلی چون درک داده‌ها، پاکسازی و آماده‌سازی، انجام تحلیل‌های اکتشافی، مدل‌سازی (در صورت نیاز) و تفسیر نتایج خواهد بود.
از سوی دیگر، این پروژه با درک چالش‌های ورود به پروژه‌های واقعی، به دنبال ایجاد فضایی امن و آموزشی برای افرادی است که هنوز در ابتدای مسیر حرفه‌ای خود قرار دارند و نیازمند تقویت اعتماد به نفس هستند. محوریت کار در این پروژه بر دو بخش اساسی استوار است: تحلیل داده به عنوان سنگ بنای کشف دانش از دل اطلاعات، و آشنایی با رویکردها و مفاهیم کلیدی در پروژه‌های علم داده که می‌توانند در پروژه‌های پیچیده‌تر مورد استفاده قرار گیرند.
با همراهی در این سفر تحلیلی، نه تنها مهارت‌های فنی خود را ارتقا خواهید داد، بلکه با چالش‌های واقعی داده‌های دنیای کسب‌وکار نیز آشنا خواهید شد و گامی محکم‌تر به سوی تبدیل شدن به یک متخصص داده برخواهید داشت.

 ##  دانلود فایل مورد استفاده در پروژه : 
 [مجموعه داده تبلیغات املاک دیوار](https://huggingface.co/datasets/divaroffical/real_estate_ads)

*	استخراج داده ها از هاگین فیس 
*	انتقال داده ها به SQL Server 
*	تجزیه و تحلیل اولیه داده ها در SQL 
*	وصل کردن داده های درج شده در SQL به پایتون 
*	EDA پایتون 
*	انتخاب ویژگی 
*	تولید ویژگی (ایجاد ویژگی های جدید) 
*	گزارش اول برای تمام داده ها 
*	پاکسازی داده ها 
*	ایجاد مدل ها 
*	نمایش نمودارها در Power BI 
*	نصب Power BI 
*	وارد کردن داده ها به عنوان SQL Servers 
*	ایجاد داشبورد جدید 
* نوشتن گزارش 
*	ارائه 
*	مهلت: 1 خرداد 1404

# 📊 Schema
The dataset includes comprehensive property information organized in the following categories:

### 🏷️ Categorization
cat2_slug, cat3_slug: Property categorization slugs
property_type: Type of property (apartment, villa, land, etc.)
### 📍 Location
city_slug, neighborhood_slug: Location identifiers
location_latitude, location_longitude: Geographic coordinates
location_radius: Location accuracy radius
### 📝 Listing Details
created_at_month: Timestamp of when the ad was created
user_type: Type of user who posted the listing (individual, agency, etc.)
description, title: Textual information about the property
### 💰 Financial Information
Rent-related: rent_mode, rent_value, rent_to_single, rent_type
Price-related: price_mode, price_value
Credit-related: credit_mode, credit_value
Transformed values: Various transformed financial metrics for analysis
### 🏢 Property Specifications
land_size, building_size: Property dimensions (in square meters)
deed_type, has_business_deed: Legal property information
floor, rooms_count, total_floors_count, unit_per_floor: Building structure details
construction_year, is_rebuilt: Age and renovation status
### 🛋️ Amenities and Features
Utilities: has_water, has_electricity, has_gas
Climate control: has_heating_system, has_cooling_system
Facilities: has_balcony, has_elevator, has_warehouse, has_parking
Luxury features: has_pool, has_jacuzzi, has_sauna
Other features: has_security_guard, has_barbecue, building_direction, floor_material
### 🏨 Short-term Rental Information
regular_person_capacity, extra_person_capacity
cost_per_extra_person
Pricing variations: rent_price_on_regular_days, rent_price_on_special_days, rent_price_at_weekends