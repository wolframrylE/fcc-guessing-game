--
-- PostgreSQL database dump
--

-- Dumped from database version 12.17 (Ubuntu 12.17-1.pgdg22.04+1)
-- Dumped by pg_dump version 12.17 (Ubuntu 12.17-1.pgdg22.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE number_guess;
--
-- Name: number_guess; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE number_guess WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE number_guess OWNER TO freecodecamp;

\connect number_guess

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: users; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.users (
    username character varying(22) NOT NULL,
    games_played integer DEFAULT 0,
    best_game integer DEFAULT 1000
);


ALTER TABLE public.users OWNER TO freecodecamp;

--
-- Data for Name: users; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.users VALUES ('user_1738398634166', 2, 472);
INSERT INTO public.users VALUES ('user_1738398996105', 2, 75);
INSERT INTO public.users VALUES ('user_1738398634167', 5, 170);
INSERT INTO public.users VALUES ('user_1738398996106', 5, 404);
INSERT INTO public.users VALUES ('user_1738398653902', 2, 676);
INSERT INTO public.users VALUES ('user_1738398653903', 5, 632);
INSERT INTO public.users VALUES ('user_1738399066423', 2, 916);
INSERT INTO public.users VALUES ('user_1738398713523', 2, 157);
INSERT INTO public.users VALUES ('user_1738399066424', 5, 124);
INSERT INTO public.users VALUES ('user_1738398713524', 5, 122);
INSERT INTO public.users VALUES ('user_1738398812478', 2, 556);
INSERT INTO public.users VALUES ('user_1738398812479', 5, 44);
INSERT INTO public.users VALUES ('user_1738398883610', 2, 4);
INSERT INTO public.users VALUES ('user_1738398883611', 5, 53);
INSERT INTO public.users VALUES ('user_1738398926902', 2, 286);
INSERT INTO public.users VALUES ('user_1738398926903', 5, 430);
INSERT INTO public.users VALUES ('user_1738398948962', 2, 347);
INSERT INTO public.users VALUES ('user_1738398948963', 5, 59);
INSERT INTO public.users VALUES ('user_1738398973856', 2, 21);
INSERT INTO public.users VALUES ('user_1738398973857', 5, 470);


--
-- Name: users users_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.users
    ADD CONSTRAINT users_pkey PRIMARY KEY (username);


--
-- PostgreSQL database dump complete
--

