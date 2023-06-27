Deception technology
===========================================

With deception technology, the environment is populated with decoys: fake endpoints, files, services, databases, users, computers, and other resources that mimic assets. The intent is to lure adversaries away from legitimate targets and detect intruders in the early stages of an attack, both key to minimising damage.

A honeypot is a deliberately vulnerable security tool designed to attract attackers and record the actions of adversaries. Honeypots can be used in production in a defensive role to alert administrators of potential breaches and to distract attackers away from real infrastructure. Honeypots can also be used for researching PTTs (procedures, tools and techniques) of adversaries and assist with generating effective defensive measures.

.. toctree::
   :maxdepth: 1
   :includehidden:
   :caption: Notes

   docs/notes/README.md
   docs/notes/taxonomies.md
   docs/notes/roadmaps.md
   docs/notes/concealed.md
   docs/notes/detection.md

.. toctree::
   :maxdepth: 1
   :includehidden:
   :caption: Deployment

   docs/deploy/README.md
   docs/deploy/tpot.md
   docs/deploy/cowrie.md
   docs/deploy/greedybear.md

----

.. toctree::
   :maxdepth: 1
   :includehidden:
   :caption: Keeping an eye on

   Thug <https://github.com/buffer/thug>
   Conpot <https://github.com/mushorg/conpot>
   Glutton <https://github.com/mushorg/glutton>
   Snare and Tanner <https://github.com/mushorg/tanner>
   OWASP’s Honeypot Project <https://owasp.org/www-project-honeypot/>


----

Books
---------------------------

.. card-carousel:: 3

    .. card::
        :link: https://chrissanders.org/2020/09/idh-release/

        .. image:: _static/images/bookcovers/sanders-honeypots.png

    .. card::
        :link: https://www.routledge.com/Implementing-Enterprise-Cybersecurity-with-Opensource-Software-and-Standard/Handa-Negi-Shukla/p/book/9788770224239

        .. image:: _static/images/bookcovers/enterprise-cyber-security.png

    .. card::
        :link: https://www.routledge.com/Real-Life-Applications-of-the-Internet-of-Things-Challenges-Applications/Mangla-Kumar-Mehta-Bhushan-Mohanty/p/book/9781774638477

        .. image:: _static/images/bookcovers/real-life-iot.png

    .. card::
        :link: https://www.packtpub.com/product/network-security-strategies/9781789806298

        .. image:: _static/images/bookcovers/network-security-strategies.png
