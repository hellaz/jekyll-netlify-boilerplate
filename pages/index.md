---
layout: home
title: Welcome
permalink: /
section: home
intro_paragraph: "[Jekyll Netlify
  Boilerplate](https://github.com/danurbanowicz/jekyll-netlify-boilerplate)
  provides the basics to get a fast, static website deployed on Netlify."
---
<head>
    <meta charset="utf-8">
    <link rel="icon" type="image/x-icon" href="/favicon.ico"/>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="robots" content="follow,index">
    <META NAME="Title" CONTENT="Public Cloud Service Index Comparison | AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <META NAME="Keywords" CONTENT="AWS vs Azure vs Google vs IBM vs Oracle Cloud vs Alibaba, AWS vs Azure, Azure vs Google, AWS vs Oracle, Oracle vs Good,">
    <META NAME="Description" CONTENT="A public cloud services comparison & mapping of Amazon AWS, Microsoft Azure, Google Cloud, IBM Cloud, Oracle Cloud.">
    <META NAME="Author" CONTENT="NEtZ">
    <META NAME="Subject" CONTENT="Public Cloud Service Comparison > AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <meta property="og:type" content="website">
    <meta property="og:title" content="Public Cloud Service Comparison > AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <meta property="og:locale" content="en_US">
    <meta property="og:description" content="A detailed public cloud services comparison & mapping of Amazon AWS, Microsoft Azure, Google Cloud, IBM Cloud, Oracle Cloud.">
    <link rel="canonical" href="https://comparecloud.in/">
    <meta property="og:url" content="https://comparecloud.in/">
    <meta property="og:site_name" content="Public Cloud Service Comparison > AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <meta property="og:image" content="/img/Logo_small.jpg">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:site" content="@">
    <meta name="twitter:creator" content="@">
    <meta property="article:author" content="https://www.facebook.com/sitez.GR">
    <meta name="twitter:description" content="A detailed public cloud services comparison & mapping of Amazon AWS, Microsoft Azure, Google Cloud, IBM Cloud, Oracle Cloud.">
    <meta name="twitter:title" content="A public Cloud Compareison : AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <title>AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba | A detailed comparison and mapping between various cloud services</title>
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-3269987799484354"
     crossorigin="anonymous"></script>
</head>
<script type="text/javascript" src="//s7.addthis.com/js/300/addthis_widget.js#pubid=ra-552c144e4f497fe9"></script>
<!-- Place this tag in your head or just before your close body tag. -->
<script async defer src="https://buttons.github.io/buttons.js"></script>

<table id="comparison">
  <tr align="center" class="header">
	            <th style="width:7%">Category</th>
            <th style="width:10%">Service</th>
            <th>
              <img  src="https://pbs.twimg.com/profile_images/1388165108786884619/ZnSwt6Qb_400x400.jpg" alt="Amazon AWS" width="100" class="header-img"/>
            </th>
            <th>
              <img  src="https://pbs.twimg.com/profile_images/1268207800313774080/KF9pXfXU_400x400.jpg" alt="Microsoft Azure Cloud" width="100" class="header-img"/>
            </th>
            <th>
              <img  src="https://pbs.twimg.com/profile_images/1190319303041724417/1a61e4pu_400x400.jpg" alt="Google Cloud Platform Logo" width="100" class="header-img" />
            </th>
            <th>
              <img  src="https://pbs.twimg.com/profile_images/1367195110224650242/RCjpV_cA_400x400.jpg"  alt="IBM Cloud Logo" width="100" class="header-img" />
            </th>
            <th>
              <img  src="https://pbs.twimg.com/profile_images/1171372058892283904/tYAN0C0c_400x400.jpg" alt="Oracle Cloud Logo" width="100" class="header-img"/>
            </th>
            <th>
              <img src="https://pbs.twimg.com/profile_images/1108554736398004224/Za8pS-nr_400x400.png" alt="Alibaba Cloud Logo" width="100" class="header-img"/>
            </th>
			<th>
              <img  src="https://pbs.twimg.com/profile_images/1001040049293508608/kk-AIfb4_400x400.jpg" alt="Huawei Cloud" width="100" class="header-img"/>
            </th>
  </tr>
	{% for item in site.data.cloudservices.services %}
	<tr>
		<td>{{item.category}}</td>
		<td>{{item.subcategory}}</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.aws %}
						<li ><img src="/assets/img/cloudproviders/aws/{{record.icon}}" alt="{{record.name}}" > <a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.azure %}
						<li><img src="/assets/img/cloudproviders/azure/{{record.icon}}" alt="{{record.name}}"  ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
				{% for record in entry.google %}
					<li><img src="/assets/img/cloudproviders/google/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
				{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
				{% for record in entry.ibm %}
						<li><img src="/assets/img/cloudproviders/ibm/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
				{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.oracle %}
							<li ><img src="/assets/img/cloudproviders/oracle/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.alibaba %}
							<li><img src="/assets/img/cloudproviders/alibaba/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.huawei %}
							<li>
								<img src="/assets/img/cloudproviders/huawei/{{record.icon}}" alt="{{record.name}}">
								<a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a>
							</li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
	</tr>
	{% endfor %}
</table>
