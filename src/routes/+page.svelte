<script>
  import { onMount } from 'svelte';

  let language = 'en';

  onMount(() => {
    const savedLanguage = localStorage.getItem('language');
    language = savedLanguage === 'de' ? 'de' : 'en';
    document.documentElement.lang = language;
  });

  function setLanguage(nextLanguage) {
    language = nextLanguage;
    localStorage.setItem('language', language);
    document.documentElement.lang = language;
  }

  const github = 'https://github.com/sukanyanath1';

  const scholar =
    'https://scholar.google.com/citations?user=WWjzvnoAAAAJ&hl=en';

  const linkedin = 'https://www.linkedin.com/in/sukanyanath/';

  const email = 'mailto:sukanyanath6@gmail.com';

  const presentations = [
    {
      title: 'Agentic Chatbot Architecture',
      previewUrl:
        '/presentations/Informationskiosk_Seminar_published_slides.pdf#page=1&view=FitH&toolbar=0',
      url: '/presentations/Informationskiosk_Seminar_published_slides.pdf'
    },
    {
      title: 'Basics of Generative AI - Under the Hood',
      previewUrl:
        'https://docs.google.com/presentation/d/1hrMPllIGBMJaxSiCayg3VY4-FPf7IhHB65coL120kPQ/embed?start=false&loop=false&delayms=3000',
      url: 'https://docs.google.com/presentation/d/1hrMPllIGBMJaxSiCayg3VY4-FPf7IhHB65coL120kPQ/edit?usp=sharing'
    },
    {
      title: 'Web Scraping',
      previewUrl:
        'https://docs.google.com/presentation/d/10wctaEvJ0aplVyQNwYEFFI5lSGPgPRJqgNdrUfWVmCs/embed?start=false&loop=false&delayms=3000',
      url: 'https://docs.google.com/presentation/d/10wctaEvJ0aplVyQNwYEFFI5lSGPgPRJqgNdrUfWVmCs/edit?usp=sharing'
    },
    {
      title: 'AI Anwendungen im administrativen Bereich',
      previewUrl:
        '/presentations/AI%20Anwendungen%20im%20administrativen%20Bereich.pdf#page=1&view=FitH&toolbar=0',
      url: '/presentations/AI%20Anwendungen%20im%20administrativen%20Bereich.pdf'
    },
    {
      title: 'NLP and Digital Traces',
      previewUrl:
        '/presentations/01_Introduction%20to%20NLP.pdf#page=1&view=FitH&toolbar=0',
      url: '/presentations/01_Introduction%20to%20NLP.pdf'
    }
  ];

  const projects = [
    {
      title: 'Generative AI Platform / Bot-as-a-Service',
      description:
        'A reusable platform for deploying customer-specific RAG and agentic AI applications, with tenant-specific configuration, retrieval infrastructure, authentication, evaluation and deployment tooling.',
      role:
        'Architecture and implementation across the AI backend, retrieval layer, customer configuration, deployment infrastructure and evaluation.',
      technologies: [
        'Python',
        'FastAPI',
        'Azure AI Search',
        'RAG',
        'Agentic AI',
        'Redis',
        'Kubernetes',
        'Terraform'
      ],
      links: [
        {
          label: 'Live Site',
          url: 'http://baas.dsl.unibe.ch'
        },
        {
          label: 'GitHub',
          url: github
        }
      ]
    },
    {
      title: 'InformationsKiosk - University Information Assistant',
      description:
        'A multilingual AI assistant for answering institutional questions using verifiable university sources. The system combines retrieval, document ingestion, source attribution, evaluation, feedback and administrative tooling.',
      role:
        'Lead development across system architecture, RAG, backend APIs, evaluation, observability and productionisation.',
      technologies: [
        'LLMs',
        'RAG',
        'FastAPI',
        'Azure',
        'SvelteKit',
        'Document Processing',
        'Evaluation',
        'Playwright'
      ],
      links: [
        {
          label: 'Live Site',
          url: 'https://informationskiosk.unibe.ch'
        },
        {
          label: 'Presentation',
          url: '/presentations/Informationskiosk_Seminar_published_slides.pdf'
        },
        {
          label: 'GitHub',
          url: github
        }
      ]
    },
    {
      title: 'CLIM+ Climate Assistant',
      description:
        'AI-powered information retrieval and question answering for climate-science content, combining web and document ingestion with retrieval and conversational access to project knowledge.',
      role:
        'Designed and implemented the retrieval, ingestion and application architecture.',
      technologies: [
        'Python',
        'Generative AI',
        'RAG',
        'Web Crawling',
        'Information Retrieval'
      ],
      links: [
        {
          label: 'Live Site',
          url: 'https://climebot.dsl.unibe.ch/'
        },
        {
          label: 'GitHub',
          url: github
        }
      ]
    },
    {
      title: 'Autonomous Research Systems',
      description:
        'Research on independently verifiable evidence for detecting epistemic degradation in autonomous research systems, including failure taxonomies, evaluation design and audit-oriented observability.',
      role:
        'Independent research and benchmark design.',
      technologies: [
        'AI Evaluation',
        'Autonomous Agents',
        'Observability',
        'Research Automation'
      ],
      links: [
        {
          label: 'Presentation',
          url: '/presentations/Autonomous%20Research%20Systems%20KPM%20and%20Med%20Libary.pdf'
        }
        
      ]
    }
  ];

  const skillGroups = [
    {
      title: 'Generative AI',
      items: [
        'RAG',
        'Agentic systems',
        'LLM evaluation',
        'Tool use',
        'Prompt and system design',
        'Grounded generation'
      ]
    },
    {
      title: 'AI & NLP',
      items: [
        'Python',
        'Natural Language Processing',
        'Transformers',
        'Machine Learning',
        'Information Retrieval',
      ]
    },
    {
      title: 'Cloud & Platform',
      items: [
        'Azure',
        'Kubernetes',
        'Docker',
        'Terraform',
        'API Management',
        'Entra ID',
        'CI/CD',
        'Apache Kafka',
        'Redis'
      ]
    },
    {
      title: 'Production Engineering',
      items: [
        'FastAPI',
        'Django',
        'Testing',
        'Observability',
        'Security',
        'Multi-tenancy',
        'System architecture'
      ]
    }
  ];

  const education = [
    {
      degree: "Bachelor's degree",
      field: 'Computer Science and Engineering',
      institution: 'NIT Silchar, India',
      year: '2009 - 2013',
    },
    {
      degree: "Master's degree",
      field: 'Computer Science (Specialization in Data Science)',
      institution: 'University of Bern',
      year: '2016 - 2018',
    },
    {
      degree: 'PhD',
      field: 'Computer Science (NLP/ Computational Linguistics)',
      institution: 'University of Neuchâtel',
      year: '2018 - 2021',
    }
  ];

  const publications = [
    {
      title:
        'Using Natural Language Processing to Find Indications for Burnout with Text Classification: From Online Data to Real-World Data',
      url: 'https://scholar.google.com/citations?view_op=view_citation&hl=en&user=WWjzvnoAAAAJ&authuser=1&citation_for_view=WWjzvnoAAAAJ:qjMakFHDy7sC'
    },
    {
      title:
        'Style change detection using Siamese neural networks',
      url:'https://scholar.google.com/citations?view_op=view_citation&hl=en&user=WWjzvnoAAAAJ&authuser=1&citation_for_view=WWjzvnoAAAAJ:u-x6o8ySG0sC'
    },
    {
      title:
        'Burnoutwords-detecting burnout for a clinical setting',
        url: 'https://scholar.google.com/citations?view_op=view_citation&hl=en&user=WWjzvnoAAAAJ&authuser=1&citation_for_view=WWjzvnoAAAAJ:d1gkVwhDpl0C'
    },
    {
      title:
        'Analysis of process data to advance computer-based assessments in multilingual contexts',
        url: 'https://scholar.google.com/citations?view_op=view_citation&hl=en&user=WWjzvnoAAAAJ&authuser=1&citation_for_view=WWjzvnoAAAAJ:Tyk-4Ss8FVUC'
    }
  ];

    const germanPresentationTitles = [
      'Architektur eines agentischen Chatbots',
      'Grundlagen generativer KI - under the Hood',
      'Web Scraping',
      'KI-Anwendungen im administrativen Bereich',
      'NLP und digitale Spuren'
    ];

    const germanProjectContent = [
      {
        title: 'Generative-AI-Plattform / Bot-as-a-Service',
        description:
          'Eine wiederverwendbare Plattform zur Bereitstellung kundenspezifischer RAG- und agentischer KI-Anwendungen mit mandantenspezifischer Konfiguration, Retrieval-Infrastruktur, Authentifizierung, Evaluation und Deployment-Werkzeugen.',
        role:
          'Architektur und Implementierung von KI-Backend, Retrieval-Schicht, Kundenkonfiguration, Deployment-Infrastruktur und Evaluation.',
        technologies: [
          'Python', 'FastAPI', 'Azure AI Search', 'RAG', 'Agentische KI',
          'Redis', 'Kubernetes', 'Terraform'
        ]
      },
      {
        title: 'InformationsKiosk - Universitärer Informationsassistent',
        description:
          'Ein mehrsprachiger KI-Assistent zur Beantwortung institutioneller Fragen anhand überprüfbarer universitärer Quellen. Das System verbindet Retrieval, Dokumentenaufnahme, Quellenangaben, Evaluation, Feedback und Administrationswerkzeuge.',
        role:
          'Technische Leitung für Systemarchitektur, RAG, Backend-APIs, Evaluation, Observability und Produktivsetzung.',
        technologies: [
          'LLMs', 'RAG', 'FastAPI', 'Azure', 'SvelteKit',
          'Dokumentenverarbeitung', 'Evaluation', 'Playwright'
        ]
      },
      {
        title: 'CLIM+ Klimaassistent',
        description:
          'KI-gestützte Informationssuche und Fragebeantwortung für klimawissenschaftliche Inhalte. Web- und Dokumentenaufnahme werden mit Retrieval und dialogischem Zugriff auf Projektwissen verbunden.',
        role:
          'Konzeption und Implementierung der Retrieval-, Ingestion- und Anwendungsarchitektur.',
        technologies: [
          'Python', 'Generative KI', 'RAG', 'Web Crawling', 'Information Retrieval'
        ]
      },
      {
        title: 'Autonomous Research Systems',
        description:
          'Forschung zu unabhängig überprüfbarer Evidenz für die Erkennung epistemischer Verschlechterung in autonomous Research Systems, einschliesslich Fehlertaxonomien, Evaluationsdesign und audit-orientierter Observability.',
        role: 'Unabhängige Forschung und Benchmark-Design.',
        technologies: [
          'KI-Evaluation', 'Autonome Agenten', 'Observability', 'Forschungsautomatisierung'
        ]
      }
    ];

    const germanSkillGroups = [
      {
        title: 'Generative KI',
        items: [
          'RAG', 'Agentische Systeme', 'LLM-Evaluation', 'Werkzeugnutzung',
          'Prompt- und Systemdesign', 'Quellengestützte Generierung'
        ]
      },
      {
        title: 'KI & NLP',
        items: [
          'Python', 'Natural Language Processing', 'Transformers',
          'Maschinelles Lernen', 'Information Retrieval'
        ]
      },
      {
        title: 'Cloud & Plattform',
        items: [
          'Azure', 'Kubernetes', 'Docker', 'Terraform', 'API Management',
          'Entra ID', 'CI/CD', 'Apache Kafka', 'Redis'
        ]
      },
      {
        title: 'Produktionsentwicklung',
        items: [
          'FastAPI', 'Django', 'Tests', 'Observability', 'Sicherheit',
          'Mandantenfähigkeit', 'Systemarchitektur'
        ]
      }
    ];

    const germanEducation = education.map((item, index) => ({
      ...item,
      degree: ['Bachelorabschluss', 'Masterabschluss', 'PhD'][index],
      field: [
        'Informatik und Ingenieurwesen',
        'Informatik (Spezialisierung Data Science)',
        'Informatik (NLP / Computerlinguistik)'
      ][index],
      institution: [
        'NIT Silchar, Indien',
        'Universität Bern',
        'Universität Neuenburg'
      ][index]
    }));

    const copy = {
      en: {
        languageLabel: 'Language',
        nav: ['Work', 'Engineering', 'Independent Advisory', 'Research', 'About'],
        heroTitle: 'I build AI systems from prototype to production.',
        heroCopy:
          'AI and NLP engineer working across Generative AI, retrieval, agentic workflows, evaluation and cloud infrastructure. I design systems from architecture and implementation through deployment, observability and operation.',
        email: 'Email',
        introBefore: 'I work at the intersection of',
        introStrong: 'AI research and production software engineering',
        introAfter:
          'My work ranges from NLP and machine-learning research to reusable Generative AI platforms, retrieval systems and applications used in real organisational environments.',
        workHeading: 'Selected Work',
        roleLabel: 'My role:',
        engineeringHeading: 'Engineering',
        advisoryHeading: 'Independent Advisory',
        advisoryLead:
          'I am available for selected independent advisory engagements in Generative AI, NLP and production AI systems.',
        advisoryNote:
          'Engagements are considered on a limited basis and subject to compatibility with my existing professional responsibilities.',
        advisoryTypes: 'Typical engagements',
        advisoryItems: [
          { title: 'AI architecture reviews for RAG, agentic and cloud-based AI systems' },
          {
            title: 'Tailored Workshops & Expert Sessions',
            description: 'Focused technical sessions on Generative AI, RAG, agentic systems, NLP, AI evaluation and production AI engineering.'
          },
          { title: 'Second opinions on AI system design, harnesses and technology choices' },
          { title: 'AI and Agentic Workflow Evaluations and observability reviews' },
          { title: "Co Supervision of master's theses" },
          { title: 'Guidance on how to convert your research problem to a concrete project' }
        ],
        contactHeading: 'Get in touch',
        contactCopy: 'Have a project or workshop in mind? Get in touch',
        emailMe: 'Email me',
        universityProfile: 'University profile',
        researchHeading: 'Research',
        researchCopy:
          'My research background is in Natural Language Processing and applied machine learning. My current interests include Generative AI, autonomous research systems, AI evaluation and the reliability of AI-assisted scientific workflows.',
        publicationLink: 'Full publication list on Google Scholar',
        selectedPublications: 'Selected publications',
        teachingHeading: 'Teaching & Training',
        teachingBefore:
          'I teach modern NLP and Transformers and contribute to technical training in AI, machine learning and research software engineering. I particularly enjoy translating emerging AI methods into systems and practices that other researchers and engineers can use. In addition to the selected presentations, I am also a module lecturer for the',
        teachingLink: 'CAS in Natural Language Processing',
        aboutHeading: 'About',
        aboutProfile: 'University of Bern profile',
        aboutLocation: 'I am an AI engineer and researcher based in Bern, Switzerland.',
        aboutSystems:
          'I am particularly interested in systems that need to move beyond demonstrations: AI systems that have to be evaluated, deployed, secured, observed and maintained for real users.',
        aboutWork:
          'My work combines machine learning and NLP with backend engineering, cloud infrastructure and system architecture.',
        aboutFamilyBefore: 'When I am not working, I am being a',
        aboutFamilyStrong: 'mum',
        aboutFamilyAfter: 'to a curious child.',
        educationHeading: 'Education',
        footerRole: 'AI / NLP Engineer · Bern, Switzerland'
      },
      de: {
        languageLabel: 'Sprache',
        nav: ['Projekte', 'Engineering', 'Unabhängige Beratung', 'Forschung', 'Über mich'],
        heroTitle: 'Ich entwickle KI-Systeme vom Prototyp bis zur Produktion.',
        heroCopy:
          'Als KI- und NLP-Ingenieurin arbeite ich an generativer KI, Retrieval, agentischen Workflows, Evaluation und Cloud-Infrastruktur. Ich konzipiere Systeme von der Architektur und Implementierung bis zu Deployment, Observability und Betrieb.',
        email: 'E-Mail',
        introBefore: 'Ich arbeite an der Schnittstelle von',
        introStrong: 'KI-Forschung und produktiver Softwareentwicklung',
        introAfter:
          'Meine Arbeit reicht von NLP- und Machine-Learning-Forschung bis zu wiederverwendbaren Plattformen für generative KI, Retrieval-Systemen und Anwendungen im realen organisatorischen Einsatz.',
        workHeading: 'Ausgewählte Projekte',
        roleLabel: 'Meine Rolle:',
        engineeringHeading: 'Engineering',
        advisoryHeading: 'Unabhängige Beratung',
        advisoryLead:
          'Ich stehe für ausgewählte unabhängige Beratungsmandate zu generativer KI, NLP und produktiven KI-Systemen zur Verfügung.',
        advisoryNote:
          'Mandate nehme ich in begrenztem Umfang und vorbehaltlich der Vereinbarkeit mit meinen bestehenden beruflichen Verpflichtungen an.',
        advisoryTypes: 'Typische Mandate',
        advisoryItems: [
          { title: 'Architektur-Reviews für RAG-, agentische und cloudbasierte KI-Systeme' },
          {
            title: 'Massgeschneiderte Workshops & Expertensessions',
            description: 'Fokussierte technische Sessions zu generativer KI, RAG, agentischen Systemen, NLP, KI-Evaluation und produktiver KI-Entwicklung.'
          },
          { title: 'Zweitmeinungen zu KI-Systemdesign, Entwicklungsumgebungen und Technologiewahl' },
          { title: 'Evaluation agentischer KI-Workflows und Observability-Reviews' },
          { title: 'Co-Betreuung von Masterarbeiten' },
          { title: 'Beratung zur Überführung einer Forschungsfrage in ein konkretes Projekt' }
        ],
        contactHeading: 'Kontakt',
        contactCopy: 'Sie haben ein Projekt oder einen Workshop im Sinn? Schreiben Sie mir.',
        emailMe: 'E-Mail senden',
        universityProfile: 'Universitätsprofil',
        researchHeading: 'Forschung',
        researchCopy:
          'Mein Forschungshintergrund liegt in Natural Language Processing und angewandtem maschinellem Lernen. Meine aktuellen Interessen umfassen generative KI, autonome Forschungssysteme, KI-Evaluation und die Zuverlässigkeit KI-gestützter wissenschaftlicher Workflows.',
        publicationLink: 'Vollständige Publikationsliste auf Google Scholar',
        selectedPublications: 'Ausgewählte Publikationen',
        teachingHeading: 'Lehre & Weiterbildung',
        teachingBefore:
          'Ich unterrichte modernes NLP und Transformers und wirke an technischen Weiterbildungen zu KI, maschinellem Lernen und Forschungssoftware mit. Besonders gern überführe ich neue KI-Methoden in Systeme und Praktiken, die Forschende und Entwicklerinnen und Entwickler nutzen können. Neben den ausgewählten Präsentationen bin ich Moduldozentin im',
        teachingLink: 'CAS Natural Language Processing',
        aboutHeading: 'Über mich',
        aboutProfile: 'Profil der Universität Bern',
        aboutLocation: 'Ich bin KI-Ingenieurin und Forscherin und lebe in Bern, Schweiz.',
        aboutSystems:
          'Mich interessieren besonders Systeme, die über Demonstratoren hinausgehen: KI-Systeme, die für reale Nutzerinnen und Nutzer evaluiert, bereitgestellt, abgesichert, beobachtet und gewartet werden müssen.',
        aboutWork:
          'Meine Arbeit verbindet maschinelles Lernen und NLP mit Backend-Entwicklung, Cloud-Infrastruktur und Systemarchitektur.',
        aboutFamilyBefore: 'Wenn ich nicht arbeite, bin ich',
        aboutFamilyStrong: 'Mutter',
        aboutFamilyAfter: 'eines neugierigen Kindes.',
        educationHeading: 'Ausbildung',
        footerRole: 'KI- / NLP-Ingenieurin · Bern, Schweiz'
      }
    };

    $: text = copy[language];
    $: localizedPresentations = language === 'de'
      ? presentations.map((presentation, index) => ({
          ...presentation,
          title: germanPresentationTitles[index]
        }))
      : presentations;
    $: localizedProjects = language === 'de'
      ? projects.map((project, index) => ({
          ...project,
          ...germanProjectContent[index],
          links: project.links.map((link) => ({
            ...link,
            label: link.label === 'Live Site'
              ? 'Live-Site'
              : link.label === 'Presentation' ? 'Präsentation' : link.label
          }))
        }))
      : projects;
    $: localizedSkillGroups = language === 'de' ? germanSkillGroups : skillGroups;
    $: localizedEducation = language === 'de' ? germanEducation : education;
</script>

<main>
  <nav class="nav container">
    <a href="/" class="brand">
      <img src="/logo.png" alt="Sukanya Nath" width="52" height="52" />
    </a>

    <div class="nav-controls">
      <div class="nav-links">
        <a href="#work">{text.nav[0]}</a>
        <a href="#engineering">{text.nav[1]}</a>
        <a href="#advisory">{text.nav[2]}</a>
        <a href="#research">{text.nav[3]}</a>
        <a href="#about">{text.nav[4]}</a>
      </div>

      <div class="language-toggle" aria-label={text.languageLabel}>
        <button
          class:active={language === 'en'}
          type="button"
          aria-pressed={language === 'en'}
          on:click={() => setLanguage('en')}
        >EN</button>
        <button
          class:active={language === 'de'}
          type="button"
          aria-pressed={language === 'de'}
          on:click={() => setLanguage('de')}
        >DE</button>
      </div>
    </div>
  </nav>

  <section class="hero container">
    <div class="eyebrow">AI/ ML ENGINEER · PhD · NLP/ GENERATIVE AI · DATA SCIENCE</div>

    <h1>Sukanya Nath</h1>

    <h2>
      {text.heroTitle}
    </h2>

    <p class="hero-copy">
      {text.heroCopy}
    </p>

    <div class="hero-links">
      <a
        class="button primary"
        href={github}
        target="_blank"
        rel="noreferrer"
      >
        GitHub
      </a>

      <a
        class="button secondary"
        href={scholar}
        target="_blank"
        rel="noreferrer"
      >
        Google Scholar
      </a>

      <a
        class="button linkedin"
        href={linkedin}
        target="_blank"
        rel="noreferrer"
      >
        LinkedIn
      </a>

      <a class="button email" href={email}>
        {text.email}
      </a>

      <!-- Add when ready:
      <a class="button secondary" href="/Sukanya_Nath_CV.pdf">
        CV
      </a>
      -->
    </div>
  </section>

  <section class="intro container">
    <p>
      {text.introBefore}
      <strong>{text.introStrong}</strong>.
      {text.introAfter}
    </p>
  </section>

  <section id="work" class="section container">
    <div class="section-heading">
      <span>01</span>
      <h2>{text.workHeading}</h2>
    </div>

    <div class="projects">
      {#each localizedProjects as project}
        <article class="project-card">
          <div class="project-main">
            <h3>{project.title}</h3>

            <p class="project-description">
              {project.description}
            </p>

            <p class="role">
              <strong>{text.roleLabel}</strong>
              {project.role}
            </p>

            <div class="tags">
              {#each project.technologies as technology}
                <span>{technology}</span>
              {/each}
            </div>
          </div>

          <div class="project-links">
            {#each project.links as link}
              <a
                href={link.url}
                target="_blank"
                rel="noreferrer"
              >
                {link.label} ↗
              </a>
            {/each}
          </div>
        </article>
      {/each}
    </div>
  </section>

  <section id="engineering" class="section container">
    <div class="section-heading">
      <span>02</span>
      <h2>{text.engineeringHeading}</h2>
    </div>

    <div class="skill-grid">
      {#each localizedSkillGroups as group}
        <article class="skill-card">
          <h3>{group.title}</h3>

          <ul>
            {#each group.items as item}
              <li>{item}</li>
            {/each}
          </ul>
        </article>
      {/each}
    </div>
  </section>

  <section id="advisory" class="section container">
    <div class="section-heading">
      <span>03</span>
      <h2>{text.advisoryHeading}</h2>
    </div>

    <div class="advisory-layout">
      <div>
        <p class="large-copy">
          {text.advisoryLead}
        </p>

        <p class="advisory-note">
          {text.advisoryNote}
        </p>
      </div>

      <div class="advisory-details">
        <h3>{text.advisoryTypes}</h3>

        <ul>
          {#each text.advisoryItems as item}
            <li>
              {item.title}
              {#if item.description}
                <p>{item.description}</p>
              {/if}
            </li>
          {/each}
        </ul>
      </div>
    </div>

    <div class="advisory-contact">
      <div>
        <h3>{text.contactHeading}</h3>
        <p>
          {text.contactCopy}
        </p>
      </div>

      <div class="advisory-actions">
        <a class="button primary" href={email}>{text.emailMe}</a>
        <a
          class="button secondary"
          href="https://www.dsl.unibe.ch/about/people_metadata/dr_nath_sukanya/"
          target="_blank"
          rel="noreferrer"
        >{text.universityProfile} ↗</a>
      </div>
    </div>
  </section>

  <section id="research" class="section container">
    <div class="section-heading">
      <span>04</span>
      <h2>{text.researchHeading}</h2>
    </div>

    <div class="research-layout">
      <div>
        <p class="large-copy">
          {text.researchCopy}
        </p>

        <a
          class="text-link"
          href={scholar}
          target="_blank"
          rel="noreferrer"
        >
          {text.publicationLink} ↗
        </a>
      </div>

      <div class="publication-list">
        <h3>{text.selectedPublications}</h3>

        {#each publications as publication}
          <article class="publication">
            <p>
              {#if publication.url}
                <a
                  class="text-link"
                  href={publication.url}
                  target="_blank"
                  rel="noreferrer"
                >{publication.title} ↗</a>
              {:else}
                {publication.title}
              {/if}
            </p>
          </article>
        {/each}
      </div>
    </div>
  </section>

  <section class="section container">
    <div class="section-heading">
      <span>05</span>
      <h2>{text.teachingHeading}</h2>
    </div>

    <p class="large-copy narrow">
      {text.teachingBefore}
      <a
        class="text-link"
        href="https://www.unibe.ch/continuing_education_programs/cas_natural_language_processing/index_eng.html#collapse_pane1290197"
        target="_blank"
        rel="noreferrer"
      >{text.teachingLink} ↗</a>.
    </p>

    <div class="presentations">
      {#each localizedPresentations as presentation}
        <article class="presentation-preview">
          <iframe
            src={presentation.previewUrl}
            title={presentation.title}
            loading="lazy"
            allowfullscreen
          ></iframe>

          <a
            class="text-link"
            href={presentation.url}
            target="_blank"
            rel="noreferrer"
          >
            {presentation.title} ↗
          </a>
        </article>
      {/each}
    </div>
  </section>

  

  <section id="about" class="section container">
    <div class="section-heading">
      <span>07</span>
      <h2>{text.aboutHeading}</h2>
    </div>

    <div class="about">
    <p>
        <a
          class="text-link"
          href="https://www.dsl.unibe.ch/about/people_metadata/dr_nath_sukanya/"
          target="_blank"
          rel="noreferrer"
        >{text.aboutProfile} ↗</a>
      </p>
      <p>
        {text.aboutLocation}
      </p>

      <p>
        {text.aboutSystems}
      </p>

      <p>
        {text.aboutWork}
      </p>
      
      <p>
        {text.aboutFamilyBefore} <strong>{text.aboutFamilyStrong}</strong> {text.aboutFamilyAfter}
      </p>

    </div>
  </section>

  <section class="education-section container">
    <div class="section-heading">
      <span>06</span>
      <h2>{text.educationHeading}</h2>
    </div>

    <div class="education-list">
      {#each localizedEducation as item}
        <article>
          <h3>{item.institution}</h3>
          <p>{item.degree} · {item.field} · {item.year}</p>
        </article>
      {/each}
    </div>
  </section>

  <footer class="footer container">
    <div>
      <strong>Sukanya Nath</strong>
      <p>{text.footerRole}</p>
    </div>

    <div class="footer-links">
      <a href={github} target="_blank" rel="noreferrer">
        GitHub
      </a>

      <a href={scholar} target="_blank" rel="noreferrer">
        Scholar
      </a>
      <a href={linkedin} target="_blank" rel="noreferrer">
        LinkedIn
      </a>
      <a href={email}>
        {text.email}
      </a>
    </div>

  </footer>
</main>