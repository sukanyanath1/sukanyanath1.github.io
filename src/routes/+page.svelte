<script>
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
</script>

<main>
  <nav class="nav container">
    <a href="/" class="brand">
      <img src="/logo.png" alt="Sukanya Nath" width="52" height="52" />
    </a>

    <div class="nav-links">
      <a href="#work">Work</a>
      <a href="#engineering">Engineering</a>
      <a href="#advisory">Independent Advisory</a>
      <a href="#research">Research</a>
      <a href="#about">About</a>
    </div>
  </nav>

  <section class="hero container">
    <div class="eyebrow">AI ENGINEERING · PhD (NLP) · GENERATIVE AI</div>

    <h1>Sukanya Nath</h1>

    <h2>
      I build AI systems from prototype to production.
    </h2>

    <p class="hero-copy">
      AI and NLP engineer working across Generative AI, retrieval,
      agentic workflows, evaluation and cloud infrastructure.
      I design systems from architecture and implementation through
      deployment, observability and operation.
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
        Email
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
      I work at the intersection of
      <strong>AI research and production software engineering</strong>.
      My work ranges from NLP and machine-learning research to reusable
      Generative AI platforms, retrieval systems and applications used
      in real organisational environments.
    </p>
  </section>

  <section id="work" class="section container">
    <div class="section-heading">
      <span>01</span>
      <h2>Selected Work</h2>
    </div>

    <div class="projects">
      {#each projects as project}
        <article class="project-card">
          <div class="project-main">
            <h3>{project.title}</h3>

            <p class="project-description">
              {project.description}
            </p>

            <p class="role">
              <strong>My role:</strong>
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
      <h2>Engineering</h2>
    </div>

    <div class="skill-grid">
      {#each skillGroups as group}
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
      <h2>Independent Advisory</h2>
    </div>

    <div class="advisory-layout">
      <div>
        <p class="large-copy">
          I am available for selected independent advisory engagements in
          Generative AI, NLP and production AI systems.
        </p>

        <p class="advisory-note">
          Engagements are considered on a limited basis and subject to
          compatibility with my existing professional responsibilities.
        </p>
      </div>

      <div class="advisory-details">
        <h3>Typical engagements</h3>

        <ul>
          <li>AI architecture reviews for RAG, agentic and cloud-based AI systems</li>
          <li> Tailored Workshops & Expert Sessions
            <p>
              Focused technical sessions on Generative AI, RAG, agentic systems, NLP, AI evaluation and production AI engineering.
            </p>
          </li>
          <li>Second opinions on AI system design, harnesses and technology choices</li>
          <li>AI and Agentic Workflow Evaluations and observability reviews</li>
          <li>Co Supervision of master's theses</li>
          <li>Guidance on how to convert your research problem to a concrete project</li>
        </ul>
      </div>
    </div>

    <div class="advisory-contact">
      <div>
        <h3>Get in touch</h3>
        <p>
          Have a project or workshop in mind? Get in touch
        </p>
      </div>

      <div class="advisory-actions">
        <a class="button primary" href="mailto:sukanyanath6@gmail.com">Email me</a>
        <a
          class="button secondary"
          href="https://www.dsl.unibe.ch/about/people_metadata/dr_nath_sukanya/"
          target="_blank"
          rel="noreferrer"
        >University profile ↗</a>
      </div>
    </div>
  </section>

  <section id="research" class="section container">
    <div class="section-heading">
      <span>04</span>
      <h2>Research</h2>
    </div>

    <div class="research-layout">
      <div>
        <p class="large-copy">
          My research background is in Natural Language Processing and
          applied machine learning. My current interests include
          Generative AI, autonomous research systems, AI evaluation and
          the reliability of AI-assisted scientific workflows.
        </p>

        <a
          class="text-link"
          href={scholar}
          target="_blank"
          rel="noreferrer"
        >
          Full publication list on Google Scholar ↗
        </a>
      </div>

      <div class="publication-list">
        <h3>Selected publications</h3>

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
      <h2>Teaching & Training</h2>
    </div>

    <p class="large-copy narrow">
      I teach modern NLP and Transformers and contribute to technical
      training in AI, machine learning and research software engineering.
      I particularly enjoy translating emerging AI methods into systems
      and practices that other researchers and engineers can use. In addition
      to the selected presentations, I am also a module lecturer for the
      <a
        class="text-link"
        href="https://www.unibe.ch/continuing_education_programs/cas_natural_language_processing/index_eng.html#collapse_pane1290197"
        target="_blank"
        rel="noreferrer"
      >CAS in Natural Language Processing ↗</a>.
    </p>

    <div class="presentations">
      {#each presentations as presentation}
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
      <h2>About</h2>
    </div>

    <div class="about">
    <p>
        <a
          class="text-link"
          href="https://www.dsl.unibe.ch/about/people_metadata/dr_nath_sukanya/"
          target="_blank"
          rel="noreferrer"
        >University of Bern profile ↗</a>
      </p>
      <p>
        I am an AI engineer and researcher based in Bern, Switzerland.
      </p>

      <p>
        I am particularly interested in systems that need to move beyond
        demonstrations: AI systems that have to be evaluated, deployed,
        secured, observed and maintained for real users.
      </p>

      <p>
        My work combines machine learning and NLP with backend
        engineering, cloud infrastructure and system architecture.
      </p>
      
      <p>
      When I am not working, I am being a <strong>mum</strong> to a curious child. 
      </p>

    </div>
  </section>

  <section class="education-section container">
    <div class="section-heading">
      <span>06</span>
      <h2>Education</h2>
    </div>

    <div class="education-list">
      {#each education as item}
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
      <p>AI / NLP Engineer · Bern, Switzerland</p>
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
        Email
      </a>
    </div>

  </footer>
</main>