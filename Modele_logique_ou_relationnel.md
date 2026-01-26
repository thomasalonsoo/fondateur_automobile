pilot(pk_pilot, name, birth_date, fk_birth_place, nationality, social_origin, training, death_date, notes)

organisation(pk_organisation, name, type, fk_headquarters_place, foundation_date, definition, notes)

occupation(pk_occupation, name, definition, notes)

event(pk_event, name, begin_date, end_date, fk_place, sources, notes)

prize(pk_prize, name, type, prize_date, fk_place, sources, notes)

contract_engagement(pk_contract_engagement, fk_pilot, fk_organisation, fk_occupation, contract_type, begin_date, end_date, sources, notes)

pilot_event(pk_pilot_event, fk_pilot, fk_event, role_in_event, sources, notes)

prize_award(pk_prize_award, fk_prize, fk_pilot, notes)

tag(pk_tag, fk_parent_tag, name, definition, notes)

pilot_tag(pk_pilot_tag, fk_pilot, fk_tag, notes)

geographical_place(pk_geographical_place, name, country, longitude, latitude, fk_geographical_place_type, notes)

geographical_place_type(pk_geographical_place_type, name, definition, fk_parent_geographical_place_type, notes)

relation_type(pk_relation_type, name, definition, notes)

pilot_relation(pk_pilot_relation, fk_pilot_source, fk_pilot_target, fk_relation_type, begin_date, end_date, sources, notes)

birth(pk_birth, fk_pilot, birth_date, fk_geographical_place, sources, notes)
