---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# To add a heading image, upload the img to /assets and type the file name + extension into "headerimg"

layout: page
headerimg: group.jpeg
tagline: Meet Our Team
heading: People
description: The AAP team consists of a diverse group of individuals from various backgrounds who share a common goal of bringing political change and upholding transparency in governance.
---
<!-- .faculty -->
<div class="container">
    <h4>State Executive Team</h4>
</div>

<div class="container-fluid mb-5 px-4">
    <div class="row limitsize">
        {% for faculty in site.data.people.faculty %}
        <div class="card-deck mx-0 p-0 col-lg-4 col-md-6">
            <a href="{{ faculty.link }}" alt="View Personal Site"><div class="card rounded-0 m-1 profile">
                <div class="row px-3">
                    <div>
                        <img src="../../assets/images/profiles/{{ faculty.img }}">
                    </div>
                    <div class="col p-3 d-flex align-items-start flex-column">
                        <h6>
                            {{ faculty.name }}
                        </h6>
                        <span class="small">
                            {{ faculty.info | newline_to_br }}
                        </span>
                        <a class="mt-auto profile-link text-right ml-auto" href="{{ faculty.link }}">
                            <span class="material-icons">
                            arrow_forward
                            </span>
                        </a>
                    </div>
                </div>
            </div></a>
        </div>
        {% endfor %}
    </div>
</div>
<!-- /.faculty -->

<!-- .postdocs -->
<div class="container mt-4">
    <h4>District Convenors</h4>
</div>

<div class="container-fluid mb-5 px-4">
    <div class="row limitsize">
        {% for postdocs in site.data.people.postdocs %}
        <div class="card-deck mx-0 p-0 col-lg-4 col-md-6">
            <a href="{{ postdocs.link }}" alt="View Personal Site"><div class="card rounded-0 m-1 profile">
                <div class="row px-3">
                    <div>
                        <img src="../../assets/images/profiles/{{ postdocs.img }}">
                    </div>
                    <div class="col p-3 d-flex align-items-start flex-column">
                        <h6>
                            {{ postdocs.name }}
                        </h6>
                        <span class="small">
                            {{ postdocs.info | newline_to_br }}
                        </span>
                        <a class="mt-auto profile-link text-right ml-auto" href="{{ postdocs.link }}">
                            <span class="material-icons">
                            arrow_forward
                            </span>
                        </a>
                    </div>
                </div>
            </div></a>
        </div>
        {% endfor %}
    </div>
</div>
<!-- /.postdocs -->

<!-- .phds -->
<div class="container mt-4">
    <h4>State Spokespersons</h4>
</div>

<div class="container-fluid mb-5 px-4">
    <div class="row limitsize">
        {% for phds in site.data.people.phds %}
        <div class="card-deck mx-0 p-0 col-lg-4 col-md-6">
            <a href="{{ phds.link }}" alt="View Personal Site"><div class="card rounded-0 m-1 profile">
                <div class="row px-3">
                    <div>
                        <img src="../../assets/images/profiles/{{ phds.img }}">
                    </div>
                    <div class="col p-3 d-flex align-items-start flex-column">
                        <h6>
                            {{ phds.name }}
                        </h6>
                        <span class="small">
                            {{ phds.info | newline_to_br }}
                        </span>
                        <a class="mt-auto profile-link text-right ml-auto" href="{{ phds.link }}">
                            <span class="material-icons">
                            arrow_forward
                            </span>
                        </a>
                    </div>
                </div>
            </div></a>
        </div>
        {% endfor %}
    </div>
</div>
<!-- /.phds -->

<!-- .mscs -->
<div class="container mt-4">
    <h4>State Social Media Team</h4>
</div>

<div class="container-fluid mb-5 px-4">
    <div class="row limitsize">
        {% for mscs in site.data.people.mscs %}
        <div class="card-deck mx-0 p-0 col-lg-4 col-md-6">
            <a href="{{ mscs.link }}" alt="View Personal Site"><div class="card rounded-0 m-1 profile">
                <div class="row px-3">
                    <div>
                        <img src="../../assets/images/profiles/{{ mscs.img }}">
                    </div>
                    <div class="col p-3 d-flex align-items-start flex-column">
                        <h6>
                            {{ mscs.name }}
                        </h6>
                        <span class="small">
                            {{ mscs.info | newline_to_br }}
                        </span>
                        <a class="mt-auto profile-link text-right ml-auto" href="{{ mscs.link }}">
                            <span class="material-icons">
                            arrow_forward
                            </span>
                        </a>
                    </div>
                </div>
            </div></a>
        </div>
        {% endfor %}
    </div>
</div>
<!-- /.mscs -->

<!-- .alumni sections -->
<div class="container-fluid bg-gray py-5 px-0">
    <!-- .faculty alumni -->
    <div class="container mt-4">
        <h4>Sundargarh Team</h4>
    </div>
    <div class="container mt-4 mb-5">
        <div class="row">
            {% for alumni-faculty in site.data.alumni.faculty %}
            <div class="col-lg-4 col-6 mb-3">
                <h6>
                    {{ alumni-faculty.name }}
                </h6>
                <span class="alumni-subheading">
                    ({{ alumni-faculty.info | newline_to_br }})
                </span>
            </div>
            {% endfor %}
        </div>
    </div>
    <!-- /.faculty alumni -->
    <!-- .postdoc alumni -->
    <div class="container mt-4">
        <h4>Balangir Team</h4>
    </div>
    <div class="container mt-4 mb-5">
        <div class="row">
            {% for alumni-postdocs in site.data.alumni.postdocs %}
            <div class="col-lg-4 col-6 mb-3">
                <h6>
                    {{ alumni-postdocs.name }}
                </h6>
                <span class="alumni-subheading">
                    ({{ alumni-postdocs.info | newline_to_br }})
                </span>
            </div>
            {% endfor %}
        </div>
    </div>
    <!-- /.postdoc alumni -->
    <!-- .phd alumni -->
    <div class="container mt-4">
        <h4>Khordha Team</h4>
    </div>
    <div class="container mt-4 mb-5">
        <div class="row">
            {% for alumni-phds in site.data.alumni.phds %}
            <div class="col-lg-4 col-6 mb-3">
                <h6>
                    {{ alumni-phds.name }}
                </h6>
                <span class="alumni-subheading">
                    ({{ alumni-phds.info | newline_to_br }})
                </span>
            </div>
            {% endfor %}
        </div>
        <h2 class="mt-3 text-right alumni-accent">...and many more!</h2>
    </div>
    <!-- /.phd alumni -->
    <!-- .msc alumni -->
    <div class="container mt-4">
        <h4>Cuttack Team</h4>
    </div>
    <div class="container mt-4 mb-5">
        <div class="row">
            {% for alumni-mscs in site.data.alumni.mscs %}
            <div class="col-lg-4 col-6 mb-3">
                <h6>
                    {{ alumni-mscs.name }}
                </h6>
                <span class="alumni-subheading">
                    ({{ alumni-mscs.info | newline_to_br }})
                </span>
            </div>
            {% endfor %}
        </div>
        <h2 class="mt-3 text-right alumni-accent">...and many more!</h2>
    </div>
    <!-- /.msc alumni -->
    <!-- .visiting alumni -->
    <div class="container mt-4">
        <h4>Sambalpur Team</h4>
    </div>
    <div class="container mt-4">
        <div class="row">
            {% for alumni-visitors in site.data.alumni.visitors %}
            <div class="col-lg-4 col-6 mb-3">
                <h6>
                    {{ alumni-visitors.name }}
                </h6>
                <span class="alumni-subheading">
                    ({{ alumni-visitors.info | newline_to_br }})
                </span>
            </div>
            {% endfor %}
        </div>
    </div>
    <!-- /.postdoc alumni -->
</div>
<!-- /.alumni sections -->
