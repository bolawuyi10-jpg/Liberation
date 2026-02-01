<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
      <title>Liberation | Access Libraries & Donate Books</title>

        <!-- Bootstrap CSS -->
          <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" />

            <!-- Leaflet (OpenStreetMap) CSS -->
              <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />

                <style>
                    :root {
                          --lib-green: #0f5132;
                                --lib-gold: #f4b400;
                                      --lib-earth: #e9f5ef;
                                            --lib-dark: #0b3d2e;
                                                }

                                                    body {
                                                          font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
                                                                line-height: 1.7;
                                                                    }

                                                                        .navbar-brand {
                                                                              font-weight: 800;
                                                                                    color: var(--lib-green) !important;
                                                                                        }

                                                                                            .hero {
                                                                                                  background: linear-gradient(135deg, var(--lib-earth), #ffffff);
                                                                                                        padding: 6rem 1rem 4rem;
                                                                                                            }

                                                                                                                .hero h1 {
                                                                                                                      color: var(--lib-green);
                                                                                                                            font-weight: 800;
                                                                                                                                }

                                                                                                                                    .map-container {
                                                                                                                                          height: 420px;
                                                                                                                                                border-radius: 16px;
                                                                                                                                                      overflow: hidden;
                                                                                                                                                            box-shadow: 0 10px 25px rgba(0,0,0,0.08);
                                                                                                                                                                }

                                                                                                                                                                    .feature-card {
                                                                                                                                                                          border-radius: 16px;
                                                                                                                                                                                border: none;
                                                                                                                                                                                      box-shadow: 0 8px 20px rgba(0,0,0,0.08);
                                                                                                                                                                                            height: 100%;
                                                                                                                                                                                                }

                                                                                                                                                                                                    footer {
                                                                                                                                                                                                          background-color: var(--lib-dark);
                                                                                                                                                                                                                color: #ffffff;
                                                                                                                                                                                                                    }

                                                                                                                                                                                                                        footer a {
                                                                                                                                                                                                                              color: #d1e7dd;
                                                                                                                                                                                                                                    text-decoration: none;
                                                                                                                                                                                                                                        }
                                                                                                                                                                                                                                          </style>
                                                                                                                                                                                                                                          </head>
                                                                                                                                                                                                                                          <body>

                                                                                                                                                                                                                                          <!-- NAVBAR -->
                                                                                                                                                                                                                                          <nav class="navbar navbar-expand-lg bg-white shadow-sm fixed-top">
                                                                                                                                                                                                                                            <div class="container">
                                                                                                                                                                                                                                                <a class="navbar-brand" href="index.html">Liberation</a>
                                                                                                                                                                                                                                                    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMenu">
                                                                                                                                                                                                                                                          <span class="navbar-toggler-icon"></span>
                                                                                                                                                                                                                                                              </button>
                                                                                                                                                                                                                                                                  <div class="collapse navbar-collapse" id="navMenu">
                                                                                                                                                                                                                                                                        <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                                                                                                                                                                                                                                                                                <li class="nav-item"><a class="nav-link" href="map.html">Map</a></li>
                                                                                                                                                                                                                                                                                        <li class="nav-item"><a class="nav-link" href="donate.html">Donate</a></li>
                                                                                                                                                                                                                                                                                                <li class="nav-item"><a class="nav-link" href="reading.html">Reading</a></li>
                                                                                                                                                                                                                                                                                                        <li class="nav-item"><a class="nav-link" href="team.html">Team</a></li>
                                                                                                                                                                                                                                                                                                                <li class="nav-item"><a class="nav-link" href="about.html">About</a></li>
                                                                                                                                                                                                                                                                                                                      </ul>
                                                                                                                                                                                                                                                                                                                          </div>
                                                                                                                                                                                                                                                                                                                            </div>
                                                                                                                                                                                                                                                                                                                            </nav>

                                                                                                                                                                                                                                                                                                                            <!-- HERO + MAP -->
                                                                                                                                                                                                                                                                                                                            <section class="hero mt-5 pt-5">
                                                                                                                                                                                                                                                                                                                              <div class="container">
                                                                                                                                                                                                                                                                                                                                  <div class="row align-items-center g-5">
                                                                                                                                                                                                                                                                                                                                        <div class="col-lg-6">
                                                                                                                                                                                                                                                                                                                                                <h1>Find Libraries. Donate Books. Support Learning.</h1>
                                                                                                                                                                                                                                                                                                                                                        <p class="lead mt-3">
                                                                                                                                                                                                                                                                                                                                                                  Liberation connects people to verified libraries and book donation centers across Nigeria — making access to knowledge easier to find, share, and support.
                                                                                                                                                                                                                                                                                                                                                                          </p>
                                                                                                                                                                                                                                                                                                                                                                                  <div class="d-flex gap-3 mt-4">
                                                                                                                                                                                                                                                                                                                                                                                            <a href="map.html" class="btn btn-success btn-lg">Find Libraries Near Me</a>
                                                                                                                                                                                                                                                                                                                                                                                                      <a href="donate.html" class="btn btn-outline-success btn-lg">Donate Books</a>
                                                                                                                                                                                                                                                                                                                                                                                                              </div>
                                                                                                                                                                                                                                                                                                                                                                                                                    </div>
                                                                                                                                                                                                                                                                                                                                                                                                                          <div class="col-lg-6">
                                                                                                                                                                                                                                                                                                                                                                                                                                  <div class="map-container" id="map"></div>
                                                                                                                                                                                                                                                                                                                                                                                                                                        </div>
                                                                                  
