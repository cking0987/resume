<template>
  <div id="app">

		<!-- Header -->
		<div class="header-container">
			<Header
			name="Charles King"
			nickname="Chuck"
			pronouns="he, him, his"
			title="UX/UI Designer &amp; Developer"
			phone="978-239-8883"
			email="cking0987@gmail.com"
			website="c9db.com" />
		</div>
		
		<!-- About -->
		<div class="about-container">
			<About
			content="UX/UI designer and front-end developer with product owner experience and certification. Detail-oriented and driven. Passionate about learning new technologies and frameworks. My goal is to create a clear and effective communications channel between organizations and their target audiences." />
		</div>

		<div class="work-skills-education">
			<!-- Work experience -->
			<div class="work-experience-container">
				<h2>Experience</h2>
				<div class="work-experience-items">
					<WorkExperience 
						jobTitle="Freelance Web Developer"
						dates="May 2017 - Present"
						employerName="Tome"
						location="NYC, NY"
						instagram="tomenyc"
						experienceDescription="Complete site redesign and migration for a fashion brand in NYC including new custom Shopify theme, new custom branded MailChimp campaign, complete product catalog reorganization. Documentation and training sessions to enable non-technical team to perform site maintenance and development."/>
					<WorkExperience 
						jobTitle="Chief of Operations"
						dates="Jan 2016 – Mar 2017"
						employerName="Bento Box"
						location="BROOKLYN, NY"
						websiteLabel="bentobox.com"
						websiteURL="https://www.bentobox.com"
						experienceDescription="Hired to help manage the growth of a fledgling startup. Very broad scope of responsibilities but key among them were product development, personnel selection and management, and website development. Set up integrated web applications to coordinate company operations all over the world (hotel booking and operation in Honolulu, Hawaii, furniture design, production and sales in Brooklyn, NY, real-estate development in Nashville, TN"/>
					<WorkExperience 
						jobTitle="Owner &amp; CEO"
						dates="DEC 2012 – JAN 2016"
						employerName="Black Market Custom"
						location="MILLBURY, MA"
						instagram="blackmarketcustom"
						experienceDescription="Started a company that designed and built custom music equipment including amplifiers and speaker cabinets. Designed, built, managed blackmarketcustom.com which functioned as an ecom site, a custom quote generator, and a products portfolio. All product photography and editing as well as company graphic design."/>
					<WorkExperience 
						jobTitle="IT Systems Admin"
						dates="JUN 2008 – DEC 2012"
						employerName="The Bioengineering Group"
						location="SALEM, MA"
						experienceDescription="Responsible for maintaining and managing IT infrastructure including multiple domains in secure environments (multiple contracts with USACE requiring military-level security protocols)."/>
				</div>
			</div>

			<!-- Skills -->
			<div class="skills-container">
				<h2>Skills</h2>
				<Skills :skills="[
					'HTML (through HTML5)',
					'CSS (through CSS3 including SASS/LESS)',
					'Adobe Suite',
					'JavaScript',
					'jQuery',
					'PHP',
					'Liquid (based on Ruby)',
					'Google Analytics',
					'WordPress',
					'Git',
					'Bootstrap'
				]"></Skills>
			</div>

			<!-- Education -->
			<div class="education-container">
				<h2>Education</h2>
				<div class="education-items">
					<Education
						major="Physics & Environmental Engineering"
						dates="JAN 2007 – MAY 2009"
						school="Suffolk University"
						location="Boston, MA"/>
					<Education
						major="Physics & Chemistry"
						dates="SEP 2006 – DEC 2006"
						school="Trinity College"
						location="Hartford, CT"/>
				</div>
			</div>
		</div>
		
		<!-- References -->
		<div class="references-container">
			<h2>References</h2>
			<div class="references-items">
				<Reference 
					name="Emily Elliott"
					phone="405-370-6330"
					email="emily.jill.elliott@gmail.com"
					title="Digital Media Consultant for TOME"
					relation="Direct manager while at TOME"
					dates="MAY 2017 – PRESENT"/>
				<Reference 
					name="Justin Koziol"
					phone="808-349-1722"
					email="jkoziol@bentobox.com"
					title="CEO, Bento Box"
					dates="JAN 2016 – MAR 2017"/>
				<Reference 
					name="Wendi Goldsmith"
					phone="617-901-2306"
					email="sustainabilityvisions@gmail.com"
					title="Owner & CEO, The Bioengineering Group "
					dates="JUN 2008 – DEC 2012"/>
			</div>
		</div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import About from './components/About.vue'
import WorkExperience from './components/WorkExperience.vue'
import Skills from './components/Skills.vue'
import Education from './components/Education'
import Reference from './components/Reference.vue'


export default {
  name: 'App',
  components: {
		Header,
		About,
		WorkExperience,
		Skills,
		Education,
		Reference
  }
}
</script>

<style>

</style>
