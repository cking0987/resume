<template>
  <div id="app">

		<!-- Header -->
		<div class="header-container">
			<Header
			name="Charles King"
			nickname="Chuck"
			pronouns="he, him, his"
			title="UX Designer &amp; Developer"
			phone="978-239-8883"
			email="cking0987@gmail.com"
			website="c9db.com" />
		</div>
		
		<!-- About -->
		<div class="about-container">
			<About
			content="I'm a UX/UI designer and front-end developer with product management experience and certification. Detail-oriented and driven, I thrive working in collaborative and energetic environments. Outside of work, I enjoy backpacking, building motorcycles, and raising my army of houseplants." />
		</div>

		<div class="work-skills-education">
			<!-- Work experience -->
			<div class="work-experience-container">
				<h2>Experience</h2>
				<div class="work-experience-items">
					<WorkExperience 
						jobTitle="Product Designer &amp; Product Owner"
						dates="DEC 2017 - Present"
						employerName="SurveyCTO (Dobility, Inc.)"
						location="Cambridge, MA"
						websiteLabel="SurveyCTO.com"
						websiteURL="https://www.surveycto.com"
						experienceDescription="Sole designer for a SaaS platform used by millions all over the world. Had to design for all levels of tech literacy (from rural farmers to data analysts) as well as for different languages, locales, and environments. Established UI design standards to unify the visual language across 2 mobile apps, a desktop app, and several web apps. As product owner, managed the prioritization and consistent release cycles of multiple apps with a tiny, resource-constrained dev team. Redesigned our user data-collection infrastructure as well as our software development lifecycle policies. Wrote all new feature specs and product documentation" />
					<WorkExperience 
						jobTitle="Freelance Web Developer"
						dates="MAY 2017 - NOV 2017"
						employerName="Tome"
						location="NYC, NY"
						instagram="tomenyc"
						experienceDescription="Digital brand identity redesign project including building a new custom Shopify theme, new MailChimp infrastructure, and documentation and training sessions to enable non-technical team to perform site maintenance and development."/>
						<!-- old description: Complete site redesign and migration for a fashion brand in NYC including new custom Shopify theme, new custom branded MailChimp campaign, complete product catalog reorganization. Documentation and training sessions to enable non-technical team to perform site maintenance and development. -->
					<WorkExperience 
						jobTitle="Chief of Operations"
						dates="Jan 2016 – Mar 2017"
						employerName="Bento Box"
						location="BROOKLYN, NY"
						websiteLabel="bentobox.com"
						websiteURL="https://www.bentobox.com"
						experienceDescription="Hired to help manage the growth of a fledgling startup. Very broad scope of responsibilities including product development, personnel selection and management, and website development. Set up integrated web apps to coordinate company operations all over the world."/>
						<!-- old description: Hired to help manage the growth of a fledgling startup. Very broad scope of responsibilities but key among them were product development, personnel selection and management, and website development. Set up integrated web applications to coordinate company operations all over the world (hotel booking and operation in Honolulu, Hawaii, furniture design, production and sales in Brooklyn, NY, real-estate development in Nashville, TN -->
					<WorkExperience 
						jobTitle="Owner &amp; CEO"
						dates="DEC 2012 – JAN 2016"
						employerName="Black Market Custom"
						location="MILLBURY, MA"
						instagram="blackmarketcustom"
						experienceDescription="Started a company that designed and built custom music equipment including tube amplifiers and speaker cabinets. Designed, built, and managed our website which functioned as an ecom site, a custom quote generator, and a portfolio for our products."/>
						<!-- old description: Started a company that designed and built custom music equipment including amplifiers and speaker cabinets. Designed, built, managed blackmarketcustom.com which functioned as an ecom site, a custom quote generator, and a products portfolio. All product photography and editing as well as company graphic design.-->
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
					'HTML/CSS/JS',
					'SASS-SCSS',
					'VueJS',
					'Electron',
					'Git',
					'Jira',
					'Sketch',
					'Adobe Suite',
					'Google Analytics',
					'Google Tag Manager',
					'MailChimp',
					'WordPress',
				]"></Skills>
				<CSPO />
			</div>

			<!-- Education -->
			<div class="education-container">
				<h2>Education</h2>
				<div class="education-items">
					<Education
						major="Physics &amp; Environmental Engineering"
						dates="JAN 2007 – MAY 2009"
						school="Suffolk University"
						location="Boston, MA"/>
					<Education
						major="Physics &amp; Chemistry"
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
					name="Chris Robert"
					title="CTO, Dobility, Inc"
					dates="DEC 2017 – PRESENT"/>
				<Reference 
					name="Emily Elliott"
					title="Digital Media Consultant, TOME"
					dates="MAY 2017 – NOV 2017"/>
				<Reference 
					name="Justin Koziol"
					title="CEO, Bento Box"
					dates="JAN 2016 – MAR 2017"/>
				<Reference 
					name="Wendi Goldsmith"
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
import CSPO from './components/CSPO.vue'
import Education from './components/Education'
import Reference from './components/Reference.vue'


export default {
  name: 'App',
  components: {
		Header,
		About,
		WorkExperience,
		Skills,
		CSPO,
		Education,
		Reference
  }
}
</script>

<style>

</style>
